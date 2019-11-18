# APIERP FACTRONICA - BOLETA DE VENTA

La API para Boleta Electrónica, tiene por Finalidad el poder generar ventas desde aplicaciones externas y enviarlas al servidor del sistema ERP Factronica.
<br>Al recibir la información la API genera el documento tributario ( Boleta Electrónica ) y lo envía por correo.
<br>La información requerida para generar la Boleta, se envía a la API utilizando variables JSON.
<br>
<br><b>ARRAY DE VARIABLES JSON PARA GENERAR BOLETA ELECTRÓNICA</b>
<br>
<br><b>TOKEN</b>
<br>Tipo de Dato: String Constante Alfanumerica 10 bytes
<br>Función: Es la llave que permite que se realize la conexión entre Sistemas Cliente/Servidor.
<br>Ejemplo: AZCJKL32X3
<br>
<br><b>RUT</b>
<br>Tipo de Dato: String Variable Alfanumerica 10 bytes
<br>Función: Corresponde al rut del cliente al cual se le está generando la venta.
<br>Ejemplo: 13432447-K  ( Sin puntos, Con guión y la K siempre en mayúsculas )
<br>
<br><b>IDCONDVENTA</b>
<br>Tipo de Dato: Int Variable Largo máximo 10
<br>Función: Indice de la condición de venta, el id se define en el sistema ERP.
<br>
<br><b>IDMEDIOPAGO</b>
<br>Tipo de Dato: Int Variable Largo máximo 10
<br>Función: Indice del medio de pago, el id se define en el sistema ERP.
<br>
<br><b>TOTAL</b>
<br>Tipo de Dato: Int Variable Largo máximo 10
<br>Función: Indice del medio de pago, el id se define en el sistema ERP.
<br>
<br><b>IDMEDIOPAGO</b>
<br>Tipo de Dato: Int Variable Largo máximo 10
<br>Función: Indice del medio de pago, el id se define en el sistema ERP.

