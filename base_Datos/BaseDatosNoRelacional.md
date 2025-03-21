# Base de datos No Relacionales🎫🎪 
---
## INTRODUCCIÓN
- En la base de datos no relacional, el esquema de datos es dinamico, no es necesario crear estructura ni esquema
- su informacion es no estructurada
- No existen JOIN entre tablas
- pueden tener distintos niveles, estas no soportan sql
#### Cuando utilizar una nosql👟
- no se requieren todas las propiedades ACID en las transacciones
- Si la estructura es muy compleja, se puede usar una nosql
- los datos no son estructurados
- se requiere un alto volumen de lectura y escritura
### Teorema CAP
Consistencia: todos los nodos se ven al mismo tiempo
Disponibilidad: no siempre se ve la misma version
Particion: se puede partir, crear particiones, si una particion no funciona, las demas si pueden seguir

### Ventajas de Nosql
- tiene un alto desempeño
- Escalabilidad horizontal
### desVentajas
- No tiene un lenguaje estandarizado
- Las transacciones no son ACID
---
## Tipos de sql
### LLaves valor
- Alto desempeño
- dentro del valor puede guardar varios registros
#### Las de documento
- funcionan como las de llave, y las llaves almacenan archivos json, donde hay mas informacion
- almacenan documento indexados
#### Orientada a grafos
- se relacionan los nodos y sus relaciones
- hay que hacer la abstraccion de qcomo sera representado el grafo
- se utiliza aristas y propiedades
#### Orientada a columnas
- lectura masiva, leen las columnas
---
# DynamoDB
es un servicio nosql de amazon, escalable, y de rendimiento rapido, es serverlees
maneja grandes volumen de datos
- indices: se tienen indices locales secundarios
- recomendable para almacenar datos de usuario como por ejemplo, marcadores. score, datos cambiables en poco tiempo

- Colecciones de datoa: se llaman tablas
- Las tuplas se llaman Items
- atributos es un dato individual de un item
- clave primaria, identificador uncio para un item dentro de una tabla
