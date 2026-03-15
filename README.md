# Validación de XML con XSD y Expresiones Regulares.
Para comprobar el funcionamiento de las expresiones he empleado regex101, esto se puede revisar en este link: https://www.awesomescreenshot.com/video/50439289?key=0711c5437ad2a4819a4eb4c77af4ede4

También he realizado una captura de pantalla probando que funcione en XSD realizado https://www.awesomescreenshot.com/video/50446670?key=624eaef8d0ed7edbc94900c80e1ed495

He realizado mi XML y XSD para la creación de una futura página para jugadores de juegos online, en especial en League Of Legends, atreves de esta web que creare en un futuro, los jugadores podrán conocer a otros de su mismo rango para poder jugar entre ellos.

Respecto a las expresiones utilizadas, he empleado las siguientes:

Nombre de Usuario: he decidido que estos deben de empezar por minúsculas [a-z] ya después he permitido que use cualquier carácter numérico o alfabético [a-zA-Z0-9] pero no otros tipos de caracteres por que nos podría dificultar a la hora de realizar búsquedas de estos, y el nombre tiene que tener de 2 a 16 caracteres {2,15}.

Email: he usado [a-zA-Z0-9._%+-]+ para pillar el nombre antes del @, ya que es el funcionamiento de los correos electrónicos.

Teléfono: Para la validación de usuarios he tomado de referencia nuestro país por ellos los números solo pueden empezar por 6 o 7, y los fijos por 9. Por eso el patrón es [679][0-9]{8}.

Código Postal: Son 5 números. Al tomar como referencia España, lo máximo que se puede llegar es a 52 (Ceuta/Melilla), por ello he limitado el primer dígito de 0 a 5.

Contraseña: Como he mostrado en la captura, limite a que mínimo fueran 8 caracteres, se ser menos, esto daría error.

He ha añadido también una restricción de tipo enumeración para el rango de los usuarios del juego League of Legends, permitiendo únicamente los siguientes valores: Bronce, Plata, Oro, Platino, Diamante, Grandmaster.
