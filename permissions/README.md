SHELL PERMISSIONS
su [usuario] : cambia de usuario al usuario especificado.
whoami : imprime el usuario actual.
groups : muestra los grupos de los cuales es parte el usuario actual.
chown [user] [file] : cambia de propietario a un archivo.
chmod 774 [file] : se otorga permisos multiples a un archivo.
chmod ugo+x [file] :se otorga permisos de ejecutar al usuario, grupo y otros.
chmod mode [file] : este comando aplica los comandos al archivo especificado.
se creo script para copiar el modo al archivo olleh.
chmod -R : el siguiente comando aplica comando recursiva
mkdir -m : use este comando para crear directorio[s] si no existen y si ademas le agregas el flag -m otorgas permisos similar a chmod.
chgrp [grupo] [file] :este comando cambia de grupo al archivo
