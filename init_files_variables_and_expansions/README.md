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

</ul>
