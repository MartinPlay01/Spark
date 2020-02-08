# YARN Command Line (Yet Another Resourse Manager)

Comando para configurar y ver información acerca del cluster de YARN: yarn

Vemos las opciones posibles

yarn -help

Listamos los nodos y sabemos cuantos contenedores se encuentran ejecutandose en cada uno de ellos

yarn node -list

Información detallada del nodo

yarn node -status NodeId

Listamos las aplicaciones del cluster

yarn application -list

Matamos la aplicación

yarn application -kill <app-id>

Debugging los logs de la aplicación

yarn logs -applicationId <app-id>


