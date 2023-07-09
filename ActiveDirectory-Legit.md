Comandos de Directorio Activo
# dsquery

dsquery user -name John*: Busca usuarios cuyo nombre comienza con "John".
# dsget

dsget user "CN=John Doe,OU=Usuarios,DC=forest,DC=dt": Obtiene información detallada sobre un usuario específico.
# dsadd

dsadd user "CN=John Doe,OU=Usuarios,DC=forest,DC=dt" -samid jdoe -upn jdoe@forest.dt -fn John -ln Doe -display "John Doe" -pwd Password1 -mustchpwd yes: Crea un nuevo usuario en el Directorio Activo.
# dsmod

dsmod user "CN=John Doe,OU=Usuarios,DC=forest,DC=dt" -disabled no: Habilita la cuenta de usuario "John Doe".
# dsrm

dsrm user "CN=John Doe,OU=Usuarios,DC=forest,DC=dt": Elimina la cuenta de usuario "John Doe".
# nltest

nltest /domain_trusts: Muestra información sobre las confianzas de dominio en el entorno.
# netstat

netstat -ano: Muestra las conexiones de red activas y los puertos escuchando en el equipo.
# gpupdate

gpupdate /force: Actualiza la configuración de la política de grupo en el equipo.
# net user

net user username: Muestra información detallada sobre un usuario específico.
# net group

net group "Grupo de Ventas": Muestra información sobre un grupo específico.
# net accounts

net accounts: Muestra la configuración de la política de cuentas en el dominio.
# net share

net share: Muestra una lista de recursos compartidos en el equipo.
# net session

net session: Muestra información sobre las sesiones de usuario activas en el equipo.
# net view

net view: Muestra una lista de recursos compartidos disponibles en la red.
# repadmin

repadmin /showrepl: Muestra información detallada sobre la replicación entre controladores de dominio.
# dfsutil

dfsutil /view \forest.dt\DFSRoot: Muestra información sobre el espacio de nombres DFS (Distributed File System) en el dominio.
# gpresult

gpresult /user username /v: Muestra el resultado de la política de grupo aplicada a un usuario específico.
# dsmod

dsmod user "CN=John Doe,OU=Usuarios,DC=forest,DC=dt" -disabled yes: Deshabilita la cuenta de usuario "John Doe".

# dcdiag

dcdiag /v: Realiza un conjunto de pruebas de diagnóstico en los controladores de dominio.
# repadmin

repadmin /syncall: Inicia una sincronización forzada de replicación entre todos los controladores de dominio.
# adfind

adfind -default -f "name=John*": Busca objetos de Directorio Activo cuyo nombre comienza con "John".
# admod

admod user "John Doe" -pwdneverexpires yes: Configura que la contraseña del usuario "John Doe" nunca caduque.
# adrestore

adrestore -r "CN=John Doe,OU=Usuarios,DC=forest,DC=dt": Restaura un objeto de Directorio Activo eliminado.
# csvde

csvde -f users.csv: Exporta los usuarios del Directorio Activo a un archivo CSV.
# ldifde

ldifde -f users.ldf -s <controlador de dominio>: Importa o exporta objetos de Directorio Activo utilizando el formato LDIF.
# repadmin

repadmin /showvector: Muestra información detallada sobre la replicación del controlador de dominio.
# dfsutil

dfsutil /purgemupcache: Borra la caché de procesamiento de política de actualización de usuario.
# gpresult

gpresult /r: Muestra el resultado de la política de grupo aplicada en el equipo.
# gpupdate

gpupdate /target:computer /wait: Actualiza la configuración de la política de grupo en el equipo y espera a que se complete.


