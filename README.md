Principios de Programación SOLID
1.	Principio de responsabilidad única: Este principio se refiere a que una clase debe tener una sola razón para cambiar. En otras palabras, la clase debe tener una única responsabilidad.
Ejemplo: Si una clase tiene dos métodos, uno para enviar correos y otro método que recibe la información de correos recibidos en este caso se estaría violando este principio ya que la clase tendría dos propósitos diferentes y si sale la necesidad de modificar alguna propiedad o procedimiento de uno de los métodos dichos cambios podrían afectar al otro método. Otro ejemplo es si una clase maneja información del usuario y también maneja la autenticación de dicho usuario, lo correcto es que se tengan dos clases separadas, una para la información y otra para la autenticación.

2.	Principio Abierto-Cerrado: Este principio consiste en que las clases deberían estar abiertas a extensión y cerradas a modificación. Básicamente, que las clases puedan ser extendidas al agregarles más información sin modificar el código ya existente de la clase ya que esto podría causar algún error. 
Ejemplo: Si tenemos una clase que imprime información a la pantalla, pero no la guarda en alguna base de datos se le podría agregar dicha funcionalidad para que guarde los datos imprimidos en alguna base de datos sin necesidad de modificar el código que ya existe. Se podría refactorizar el código de manera que obedezca el principio

3.	Principio de sustitución de Liskov: Este principio menciona que las subclases de una clase deben poder remplazar a su clase principal. Se refiere a que una subclase pueda enviar algún dato a otro método que espere información de la clase principal de la subclase.
Ejemplo: Si una subclase se encarga de realizar una suma y regresa el resultado a su clase principal esta subclase también debería poder enviar ese dato a otros métodos fuera de su clase.

4.	Principio de segregación de interfaz: Como el nombre lo dice, este principio consiste en separar interfaces. El propósito de este principio es hacer que los clientes solo vean lo que deben ver según lo que elijan y no ser forzados a usar alguna interfaz que no les sirve.
Ejemplo: En una aplicación en la que se tengan dos planes, uno gratuito y otro de paga se debe implementar que los usuarios solo vean las interfaces y funciones que les corresponde según el plan que eligieron. A los usuarios que tengan el plan gratuito no les debería aparecer alguna opción de renovar su pago en su interfaz ya que no eligieron la opción de paga, solo les debería aparecer alguna opción que les permite cambiarse al plan de paga si así lo desean. A los usuarios que tengan el plan de paga deberían poder acceder a las opciones necesarias desde la interfaz según su plan de pago que eligieron.

5.	Principio de inversión de dependencia: Este principio establece que las clases y módulos de alto y bajo de nivel deben depender de abstracciones (o clases abstractas), no deberían depender de otras clases o funciones en específico.
Ejemplo: Un ejemplo de este principio aplicado correctamente es cuando una clase que consiste en enviar alertas a usuarios dependa de una interfaz abstracta y no de una clase en específico ya que al depender de una interfaz y no de una clase no puede haber errores si se realiza algún cambio en la clase en específico para que no le afecte a la clase de las alertas.



Principios de Programación Orientada a Objetos
•	Abstracción: Este principio consiste en ser simples, que las clases deben simplificarse y solo tener lo que es relevante para lo que se quiere lograr con la clase evitando detalles innecesarios.
Ejemplo: En C# se puede tener como ejemplo el uso de clases abstractas para respetar este principio como el definir una clase abstracta cuyo único propósito sea mostrar rápidamente si un sistema está activo o inactivo.

•	Encapsulación: Es una técnica que consiste en ocultar y proteger los datos de una clase u objeto y solo se revela cierta información en específico usando métodos públicos.
Ejemplo: Un ejemplo es cuando se requiere ocultar el saldo de una cuenta bancario y se define como privada en un campo dentro de una clase.

•	Herencia: Como el nombre lo indica, es cuando las clases se definen usando otras clases heredando las propiedades y datos de las clases que se están usando para definirse. Esto permite que se reutilice código cuando una clase derivada de otra herede las propiedades de la clase base que está heredando.
Ejemplo: Si una clase requiere obtener algún dato como el nombre o edad de una persona esta puede codificarse de manera que herede dichos datos de otra clase que se encarga de tener esos datos.

•	Polimorfismo: Este principio habla del comportamiento de los métodos y como pueden ejecutarse de manera diferente según el objeto que los llame o como la aplicación los ejecuta según la instancia que llama al método.
Ejemplo: Un ejemplo de esto puede explicarse con la “Sobrecarga de métodos” que es cuando se definen dos o más métodos con el mismo nombre pero con diferentes parámetros dentro de una clase y que cuando se llame al método el programa determina cuál de los métodos ejecutar basándose en los parámetros que se le proporcionen.



Principio KISS: En ingles es "Keep it simple, stupid" que significa "Mantenlo simple, estupido". Este principio consiste en mantener el sistema y su codigo de una manera simplificada evitando complejidades como datos o informacion que sean irrelevantes y que no aporten algo al sistema o programa. Este principio ayuda a que se mantenga un codigo simple que lo hace facil de entender y mantener.

Principio DRY: En ingles es "Don't repeat yourself" que significa "No te repitas a ti mismo". Consiste en evitar la repeticion en un codigo que no necesita repetirse de manera redundante. Por ejemplo: en vez de copiar y pegar un mismo código en diferentes partes de un programa se puede analizar como funciona la lógica del codigo y crear una abstracción que puede ser una clase padre, función o método que pueda ser reutilizado.
