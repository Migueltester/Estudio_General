Contexto: Actualmente estoy creando una app neobancaria, la cual entre sus componentes y servicios, es realizar recarga a traves de escaneo de qr, entonces
Entonces, yo ya cree en la capa baja un api, que recibe el numero de cuenta y el monto, y esa api con java y springboot llama a un procedimiento almacenado sp, donde realiza transaccion
mi api solo debe recibir el numero de cuenta y el monto
entonces yo tengo un qr, esos qr cuando el usuario lo ecanea te envia un codigo
{
  "id": {
    "S": "cd8b9a7443fee8aff4f2daac885475fe"
  },
  "estado": {
    "S": "disponible"
  },
  "fecha_emision": {
    "S": "2025-03-30T05:00:00Z"
  },
  "monto": {
    "N": "200"
  }
}

ese codigo es el id

entonces,

debo crear dos lambdas, en la app el usuario escanea y eso llega a traves de un endpoint del apigateway y ahi manda al lambda ya con la informacion del cliente y la cuenta, y ese id escaneado

entonces
Lambda "Vaidar": esta lambda se encarga de validar si el estado del qr es dispoible, si esta disponible , va a permitir ejecutar la sigueinte lambda
la cual es la de "ingresar transaccion", esta lambda de validar desde tener en cuenta que el usuario escanea, entonces para cuestiones de velocidad y  no ir hasta la conexion con el api, si el qr ya ha sido utilizado, le envia una respuesta de qr ya utulizado,
tambien si si se puede utilizar, darle al usuario, aqui no se si, si esta disponible ejecuta la siguiente lambda, y le envia un mensaje de exito al user, con unos 2 o 3 segundos para que se pueda realizar la transaccion en e app. asi mismo
esa lambda debe cambiar el estado de la tabla de dynamo, de disponible a utilizado

La lambda de ingresar transaccion solo debe encargarse de ingresar al api la cuenta y el monto


aun tengo dudas de maejar respuestas, tipo si ocurre errores, seria lo ideal pero no se como hacerlo

enviame el flujo de ese y como hacer esas lambdas.
