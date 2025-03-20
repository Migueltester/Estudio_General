# Base de datos relacional
---
## Inroduccion
Sabemos que la base de datos es una representacion de informacion de una empresa
Manejadores de base de datos: es donde vas a manejar informacion y almacenarla
El DBMS es el que te permite manejar la informacion:
  - Tiene un lenguaje dedefinicion de datos
  - Tiene un lenguaje de manipulacion de datos
  - Hacer querys

## Modelos de base de datos
- Conceptuales (Diagrama E-R)
    - Entidad: 
    - Relacion
    - Atributos
- Representación (Tablas)
    - a cada row se le llama tupla
- Esquema Es donde se representan los esquemas
  ![image](https://github.com/user-attachments/assets/7a6fbc67-919b-4bc0-91c2-1beb718701a6)
- Fisico
---
## AWS RDS 
Servicio aws en la nube, servicio que administra la base de datos relacionales
  - ## Mysql:   Sistema de gestión de base de datos
  - ## Arquitectura de aws RDS mysql:
      - instancia de la base de datos
      - Almacenamiento escalable
      - Replicas de lectura
  - ## Cluster: Conjunto de base de datos
## Creacion de base de daatos (Aurora mysql)
  - Utilizamos aurora mysql ya que es mas barato y mysql necesitas licencia, tambien, al crear el cluster, se crea las instancia de escritura, entonces, crear un rds es crear un cluster, el cual almacenara las instancias, y ya podemos agregar diversas instancias de escritura y lectura

  - En rds se añade una instancia de lectura, y otra de escritura, una vez creado la base de datos y el cluster, tenemos nuestra instancia normal pero tambien podemos agregar ua instancia de escritura, en action, add reader, y listoS
  - Se pueden añadir hasta 15 servidores de lectura, solo en aurora
  - *Si ocurre un error en el servidor de escritura, un failever, este se apagara, y el que era de escritura, se volvera el de escritura, en otras palabras si se daña uno de escritura, se asignara el persmiso de escritura a uno de lectura, y ahora sera de escritura, redundiancia en su explendor pero se entendió
  - podemos asignar la preferencia de que servidor si se daña el principal de escritura, cual de lectura tomara el rol, se le asigna la prioridad.
  - Creamos una llave kms, kms service, ese arn es parahacer una copia incriptada (SNAPCHOT), Funciona para copias y de la base de datos
  - Route 53, crear hosted zone , y eso e spara manejar los endopoints de la base de datos
  - Tambien se puede crear REGION, eso es para replicar la base de datos en otra regionl, 
  - 
![image](https://github.com/user-attachments/assets/f963d15d-c3b0-4efc-b47e-06e8a6b0ffb0)

## Puntos conceptuales
- manejador de respaldo automatico por ejemplo en aws
- Los objetos tambien se pueden giardar en la base de datos
- 
