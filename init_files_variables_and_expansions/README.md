<h1>Shell, init files, variables and expansions</h1>
<ul>
<li>
    <dl>
        <dt><a href="./0-alias">alias ls="rm *"</a></dt>
        <dd><code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> alias </code> asigna un alias al comando <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> ls </code>, cada vez que ejecutemos<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> ls </code>se ejecutará <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> rm * </code></dd>
    </dl>
</li>
<li>
    <dl>
        <dt><a href="./1-hello_you">echo "hello $USER"</a></dt>
        <dd>El comando <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> echo </code> imprime por pantalla <strong>hello root</strong> suponiendo que el usuario actual sea ese,<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> $USER </code> si mostramos esta variable de entorno,nos dará el usuario actual.</dd>
    </dl>
</li>
<li>
    <dl>
        <dt><a href="./2-path">export PATH=$PATH:/action</a></dt>
        <dd>El comando <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> export </code> se usa para definir y exportar variables,para este caso estamos agregando un nuevo directorio llamado <strong> /action </strong>a la variable<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> PATH </code>.</dd>
    </dl>
</li>
<li>
    <dl>
        <dt><a href="./3-paths">echo $PATH | tr : \\n | wc -l </a></dt>
        <dd>Con esta instrucción imprimimos la cantidad de ditectorios que hay en al PATH.<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> echo $PATH </code> para mostrar los directorios que estan almacenados en la variable de entorno,luego con el pipe le pasamos la salida a la siguiente instrucción<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> tr : \\n </code> esta se encarga de reemplazar los <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> : </code> por un salto de línea y por ultimo usamos el pipe para enviar la salida a la siguiente instrucción,<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> wc -l </code> esta se encarga de contar las líneas devueltas.</dd>
    </dl>
</li>
<li>
    <dl>
        <dt><a href="./4-global_variables">env | sort </a></dt>
        <dd> Con esta instrucción mostramos las variables de entorno y las ordenamos.<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> env </code> nos sirve para mostrar los variables de entorno<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> sort </code>este comando no sirve para ordenar el contenido.</dd>
    </dl>
</li>
<li>
  <dl>
    <dt><a href="./5-local_variables">set</a></dt>
    <dd>Con este comando listamos las variables globales,locales y funciones.</dd>
  </dl>
</li>
 <li>
  <dl>
    <dt><a href="./6-create_local_variable">BEST=School</a></dt>
    <dd>Para crear una variable local lo hacemos declarando el nombre de nuestra variable y seguido asignandole el valor, para eliminar esta variable debemos usar el comando <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> unset BEST </code>.</dd>
  </dl>
</li>
 <li>
  <dl>
    <dt><a href="./7-create_global_variable">export BEST=School</a></dt>
    <dd>Para crear una variable global lo hacemos con el comando <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> export </code>  declarando el nombre de nuestra variable y seguido asignandole el valor, para eliminar esta variable debemos usar el comando <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> unset BEST </code>.</dd>
  </dl>
</li>
 <li>
  <dl>
    <dt><a href="./8-true_knowledge">echo $(($TRUEKNOWLEDGE+128))</a></dt>
    <dd>Imprimimos el resultado de la suma de 128 mas el valor de la variable TRUEKNOWLEDGE<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> echo </code>para imprimir el resultado,el signo de dolar<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> $ </code>e s para mostrar el valor de la variable y los <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> $(()) </code> para realziar la operación que esta dentro de ella .</dd>
  </dl>
</li>
 <li>
  <dl>
    <dt><a href="./9-divide_and_rule">echo $(($POWER/$DIVIDE))</a></dt>
    <dd>Imprimimos el resultado de la división de 2 variables<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> echo </code>para imprimir el resultado,el signo de dolar<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> $ </code>es para mostrar el valor de la variable y los <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> $(()) </code> para realizar la operación que esta dentro de ella .</dd>
  </dl>
</li>
 <li>
  <dl>
    <dt><a href="./10-love_exponent_breath">echo $((BREATH**LOVE))</a></dt>
    <dd>Imprimimos el resultado de exponer el valor de nuestra variable BREATH a la LOVE<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> echo </code>para imprimir el resultado,el doble asterísco <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> ** </code>se usa para trabajar con exponentes.</dd>
  </dl>
</li>

</ul>
