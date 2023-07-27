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
        <dt><a herf="./0-alias">echo "hello $(whoami)"</a></dt>
        <dd>El comando <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> echo </code> imprime por pantalla <strong>hello root</strong> suponiendo que el usuario actual sea ese,<code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> whoami </code>por si solo nos retorna el usuario actual pero como lo estamos escribiendo como argumento del comando <code style="background-color: antiquewhite; padding : 3px; border-radius:5px"> echo </code> lo encerramos de esta forma<code style="background-color: antiquewhite; padding : 3px; border-radius:5px" >$(whoami) </code>.</dd>
    </dl>
</li>
</ul>
