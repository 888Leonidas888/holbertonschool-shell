<h1>Shell, init files, variables and expansions</h1>
<ul>
<li>
    <dl>
        <dt><a herf="./0-alias">alias ls="rm *"</a></dt>
        <dd><code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> alias </code> asigna un alias al comando <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> ls </code>, cada vez que ejecutemos<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> ls </code>se ejecutará <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> rm * </code></dd>
    </dl>
</li>
<li>
    <dl>
        <dt><a herf="./1-hello_you">echo "hello $USER"</a></dt>
        <dd>El comando <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> echo </code> imprime por pantalla <strong>hello root</strong> suponiendo que el usuario actual sea ese,<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> $USER </code> si mostramos esta variable de entorno,nos dará el usuario actual.</dd>
    </dl>
</li>
<li>
    <dl>
        <dt><a herf="./2-path">export PATH=$PATH:/action</a></dt>
        <dd>El comando <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> export </code> se usa para definir y exportar variables,para este caso estamos agregando un nuevo directorio llamado <strong> /action </strong>a la variable<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> PATH </code>.</dd>
    </dl>
</li>
<li>
    <dl>
        <dt><a herf="./3-paths">echo $PATH | tr : \\n | wc -l </a></dt>
        <dd>Con esta instrucción imprimimos la cantidad de ditectorios que hay en al PATH.<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> echo $PATH </code> para mostrar los directorios que estan almacenados en la variable de entorno,luego con el pipe le pasamos la salida a la siguiente instrucción<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> tr : \\n </code> esta se encarga de reemplazar los <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> : </code> por un salto de línea y por ultimo usamos el pipe para enviar la salida a la siguiente instrucción,<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> wc -l </code> esta se encarga de contar las líneas devueltas.</dd>
    </dl>
</li>
<li>
    <dl>
        <dt><a herf="./4-global_variables">env | sort </a></dt>
        <dd> Con esta instrucción mostramos las variables de entorno y las ordenamos.<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> env </code> nos sirve para mostrar los variables de entorno<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> sort </code> <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> este comando no sirve para ordenar el contenido.</dd>
    </dl>
</li>
</ul>
