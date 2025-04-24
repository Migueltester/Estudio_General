# Aws_Practice
Practica de aws


Casos de prueba formato Gherkin

Caso 1



caso: Loguerase exitosamente con usuario y contraseña
Dado que el usuario tiene cuenta en la pagina ¨demoblazer"
Cuando  ingresa sus datos validos en el login
Entonces se validan sus datos y obtiene una respuesta exitoso
Caso 2



caso: Loguearse con usuario incorrecto
Dado que estoy en el login de la pagina "demoblazer"
Cuando ingreso un usuario invalido en el login
Entonces me devuelve error de usuario inexistente
Caso 3



Caso: Loguearse con contraseña incorrecta
Dado que estoy en el login de la pagina "demoblazer"
Cuando ingreso un usuario correcto, y contraseña invalida en el login
Entonces me devuelve error de contraseña incorrecta
Caso 4



Caso: Respuesta de las diferentes categorias phones, monitors, laptops
Dado que estoy en la pagina principal de "demoblazer"
Cuando selecciono una categoria especifica
Entonces me devuelve La lista de los distintos productos
Caso 5



Caso: Respuesta de las diferentes categorias monitors
Dado que estoy en la pagina principal de "demoblazer"
Cuando selecciono una categoria especifica
Entonces me devuelve La lista de los distintos productos
Caso 6



Caso: Respuesta de las diferentes categorias laptops
Dado que estoy en la pagina principal de "demoblazer"
Cuando selecciono una categoria especifica
Entonces me devuelve La lista de los distintos productos
 

Caso 7



Caso: Respuesta de una categoria que no existe
Dado que estoy en la pagina principal de "demoblazer"
Cuando se envia una categoria inexistente
Entonces me devuelve un error de categoria inexistente
Caso 8



Caso: Respuesta al ver los detalles del producto Sony vaio i5
Dado que el usuario esta en la categoria de "monitors"
Cuando selecciono el producto "Sony vaio i5" se envia el id del producto
Entonces me muestra los detalles del producto
Caso 9



Caso: Respuesta al ver los detalles del producto Sony vaio i7
Dado que el usuario esta en la categoria de "monitors"
Cuando selecciono el producto "Sony vaio i7" se envia el id del producto
Entonces me muestra los detalles del producto
Caso 10



Caso: Respuesta al ver los detalles del producto "MacBook air"
Dado que el usuario esta en la categoria de "monitors"
Cuando selecciono el producto "MacBook air" se envia el id del producto
Entonces me muestra los detalles del producto
Caso 11



Caso: Respuesta de producto inexistente 
Dado que el usuario esta en la categoria de "monitors"
Cuando  se envia el id del producto que no existe
Entonces me muestra los detalles del producto
Caso 12



Caso: Respuesta al agregar el producto Sony vaio i5 al carrito
Dado que el usuario esta en la categoria de "monitors"
Cuando selecciono el producto "Sony vaio i5" y lo añado al carrito
Entonces se agrega de manera exitosa
Caso 13



Caso: Respuesta al agregar el producto producto Sony vaio i7 al carrito
Dado que el usuario esta en la categoria de "monitors"
Cuando selecciono el producto "Sony vaio i7" y lo añado al carrito
Entonces se agrega de manera exitosa
Caso 14



Caso: Respuesta al agregar el producto producto "MacBook air" al carrito
Dado que el usuario esta en la categoria de "monitors"
Cuando selecciono el producto "MacBook air" y lo añado al carrito
Entonces se agrega de manera exitosa
Caso 15



Caso: Respuesta al agregar el producto que no existe al carrito
Dado que el usuario esta en la categoria de "monitors"
Cuando se le envia un producto que no existe en la base de datos
Entoncesme muestra un mensaje de error controlado
