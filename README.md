# Validación de XML con XSD y Expresiones Regulares.
Para comprobar el funcionamiento de las expresiones he empleado regex101, esto se puede revisar en este link: https://www.awesomescreenshot.com/video/50439289?key=0711c5437ad2a4819a4eb4c77af4ede4
También he realizado una captura de pantalla probando que funcione en XSD realizado https://www.awesomescreenshot.com/video/50446670?key=624eaef8d0ed7edbc94900c80e1ed495
Respecto a las expresiones utilizadas, he empleado las siguientes:
Email: he usado [a-zA-Z0-9._%+-]+ para pillar el nombre antes del @, ya que es el funcionamiento de los correos electrónicos.
Teléfono: Para la validación de usuarios he tomado de referencia nuestro país por ellos los números solo pueden empezar por 6 o 7, y los fijos por 9. Por eso el patrón es [679][0-9]{8}.
Código Postal: Son 5 números. Al tomar como referencia España, lo máximo que se puede llegar es a 52 (Ceuta/Melilla), por ello he limitado el primer dígito de 0 a 5.
Contraseña: Como he mostrado en la captura, limite a que mínimo fueran 8 caracteres, se ser menos, esto daría error.
