<h1 style='text-align:center'>IO redirections and filters</h1>

<ul>
	<li>
		<dl>
			<dt><a href='./0-hello_world'>echo</a></dt>
			<dd>Este comando sirve para imprimir una línea en la salida estandar.</dd>
		</dl> 
	</li>
	<li>
		<dl>
			<dt>cat</dt>
			<dd>Este comando sirve para mostrar el contenido de un archivo en la salida estandar.</dd>
		</dl>
	</li>
	<li>
		<dl> 
			<dt>echo "\"(Ôo)'"</dt>
			<dd>Estamos usando echo conbinando con un caracter de escape (\), para indicar que se imprima las comillas dobles (").</dd>
		</dl>
	</li>
	<li>
		<dl>
			<dt>cat /etc/passwd /etc/hosts 2>1</dt>
			<dd>Este comando lee el contenido de los archivos tanto de passwd como de hosts y los errores los muestra en la salida standar.(se reprepresenta con 0 la entrada standar,con 1 la salida standar y con 2 la salida de errores).</dd>
		</dl> 
	</li>
	<li>
		<dl>
			<dt>tail</dt>
			<dd>Este comando muestra las 10 ultimas líneas de un archivo.</dd>
		</dl>
	</li>
	<li>
		<dl>
			<dt>head</dt>
			<dd>Este comando muestra las 10 primeras líneas de un archivo</dd>
		</dl>
	</li>
	<li>
		<dl>
			<dt><a href='./6-third_line'>head -n 3 iacta | tail -n 1</a></dt>
			<dd>Este comando lee las 3 primeras líneas del archivo iacta y se las pasa como entrada estandar al comando tail que lee solo una línea</dd>
		</dl>
	</li>
	<li>
		<dl>
			<dt><a herf='./8-cwd_state'>ls -la > ls_cwd_content</a></dt>
			<dd>Este comando redirecciona la salida standar hacia un archivo llamado ls_cwd_content</dd>
		</dl>
	</li>
	<li>
		<dl>
			<dt><a href='./9-duplicate_last_line'>tail -n 1 iacta >> iacta</a></dt>
			<dd>Este comando lee la última línea del archivo iacta y redirecciona la salida estandar al archivoal mismo archivo iacta pero al usar doble signo del mayor que (>>) esta agregando al contendio del mismo.</dd>
		</dl>
	</li>
	<li>
		<dl>
			<dt><a href='./10-no_more_js'>find . -type f -name "*.js" | xargs rm</a></dt>
			<dd>Este comando busca de manera recursiva todos los archivos con estensión .js y los redirige a la entrada estandar del comando rm para que los elimine,para que rm tome el resultado del coamndo find usamos xargs.</dd> 
		</dl>
	</li>
</ul>
