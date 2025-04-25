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



---
FRONTEND

Feature: Login Functionality

  Scenario: Loguearse exitosamente con usuario y contraseña
    Given el usuario tiene cuenta en la página "demoblazer"
    When ingresa sus datos válidos en el login
    Then se validan sus datos y obtiene una respuesta exitosa

  Scenario: Loguearse con usuario incorrecto
    Given estoy en el login de la página "demoblazer"
    When ingreso un usuario inválido en el login
    Then me devuelve error de usuario inexistente

  Scenario: Loguearse con contraseña incorrecta
    Given estoy en el login de la página "demoblazer"
    When ingreso un usuario correcto y contraseña inválida en el login
    Then me devuelve error de contraseña incorrecta

Feature: Product Categories

  Scenario: Respuesta de las diferentes categorías phones, monitors, laptops
    Given estoy en la página principal de "demoblazer"
    When selecciono una categoría específica
    Then me devuelve la lista de los distintos productos

  Scenario: Respuesta de las diferentes categorías monitors
    Given estoy en la página principal de "demoblazer"
    When selecciono una categoría específica
    Then me devuelve la lista de los distintos productos

  Scenario: Respuesta de las diferentes categorías laptops
    Given estoy en la página principal de "demoblazer"
    When selecciono una categoría específica
    Then me devuelve la lista de los distintos productos

  Scenario: Respuesta de una categoría que no existe
    Given estoy en la página principal de "demoblazer"
    When se envía una categoría inexistente
    Then me devuelve un error de categoría inexistente

Feature: Product Details

  Scenario: Ver los detalles del producto Sony vaio i5
    Given el usuario está en la categoría de "monitors"
    When selecciono el producto "Sony vaio i5" y se envía el id del producto
    Then me muestra los detalles del producto

  Scenario: Ver los detalles del producto Sony vaio i7
    Given el usuario está en la categoría de "monitors"
    When selecciono el producto "Sony vaio i7" y se envía el id del producto
    Then me muestra los detalles del producto

  Scenario: Ver los detalles del producto MacBook air
    Given el usuario está en la categoría de "monitors"
    When selecciono el producto "MacBook air" y se envía el id del producto
    Then me muestra los detalles del producto

  Scenario: Ver los detalles de un producto inexistente
    Given el usuario está en la categoría de "monitors"
    When se envía el id de un producto que no existe
    Then me muestra un mensaje de error controlado

Feature: Shopping Cart

  Scenario: Agregar el producto Sony vaio i5 al carrito
    Given el usuario está en la categoría de "monitors"
    When selecciono el producto "Sony vaio i5" y lo añado al carrito
    Then se agrega de manera exitosa

  Scenario: Agregar el producto Sony vaio i7 al carrito
    Given el usuario está en la categoría de "monitors"
    When selecciono el producto "Sony vaio i7" y lo añado al carrito
    Then se agrega de manera exitosa

  Scenario: Agregar el producto MacBook air al carrito
    Given el usuario está en la categoría de "monitors"
    When selecciono el producto "MacBook air" y lo añado al carrito
    Then se agrega de manera exitosa

  Scenario: Agregar un producto inexistente al carrito
    Given el usuario está en la categoría de "monitors"
    When se envía un producto que no existe en la base de datos
    Then me muestra un mensaje de error controlado


