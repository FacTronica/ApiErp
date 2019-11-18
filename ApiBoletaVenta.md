# API ERP FACTRONICA - BOLETA DE VENTA

La API para Boleta Electrónica, tiene por Finalidad el poder generar ventas desde aplicaciones externas y enviarlas al servidor del sistema ERP Factronica.
<br>Al recibir la información la API genera el documento tributario ( Boleta Electrónica ) y lo envía por correo.
<br>La información requerida para generar la Boleta, se envía a la API utilizando variables JSON.
<br>
<br><h3><b>DATOS PARA GENERAR BOLETA ELECTRÓNICA</b></h3>
<br>
<br><b>TOKEN</b>
<br>Tipo de Dato: Obligatorio String Constante Alfanumerica 10 bytes
<br>Función: Es la llave que permite que se realize la conexión entre Sistemas Cliente/Servidor.
<br>
<br><b>TOTAL</b>
<br>Tipo de Dato: Obligatorio Int Variable Largo máximo 10
<br>Función: Indice del medio de pago, el id se define en el sistema ERP.
<br>
<br><b>CORREO</b>
<br>Tipo de Dato: Opcional Varchar Variable Largo máximo 255
<br>Función: Correo de cliente para envío de boleta electrónica.
<br>
<br><b>RUT</b>
<br>Tipo de Dato: Opcional String Variable Alfanumerica 10 bytes
<br>Función: Corresponde al rut del cliente al cual se le está generando la venta.
<br>
<br><b>IDCONDVENTA</b>
<br>Tipo de Dato: Opcional Int Variable Largo máximo 10
<br>Función: Indice de la condición de venta, el id se define en el sistema ERP.
<br>
<br><b>IDMEDIOPAGO</b>
<br>Tipo de Dato: Opcional Int Variable Largo máximo 10
<br>Función: Indice del medio de pago, el id se define en el sistema ERP.
<br>
<br><b>TIMEVCTO</b>
<br>Tipo de Dato: Opcional Int Variable Largo máximo 10
<br>Función: TimeStamp con la fecha de vencimiento de pago.
<br>
<br><b>IDVENDEDOR</b>
<br>Tipo de Dato: Opcional Int Variable Largo máximo 10
<br>Función: Indice del Vendedor, el id se define en el sistema ERP.
<br>
<br><b>IDITEM</b>
<br>Tipo de Dato: Opcional Int Variable Largo máximo 10
<br>Función: Indice del Item (Producto/Servicio), el id se define en el sistema ERP.
<br>
<br><b>OBS</b>
<br>Tipo de Dato: Opcional VarChar Variable Largo máximo 255
<br>Función: Observaciones generales o comentarios de uso interno
<br>
<br><h3><b>RETORNO DE DATOS DESDE LA API</b></h3>
<br>
<br>Si la operación fue exitosa, se retornará un valor entero, el cual corresponderá al folio de boleta electrónica generada.
<br>Se recomienda que la aplicación cliente al momento de recibir el folio de la boleta, lo almacene  y deje asociado a la venta realizada en su sistema propio.
<br>
<br><h3><b>NOTAS:</b></h3>
<br>-Al momento de generar la boleta, enviará un mail al Emisor a modo de respaldo.
<br>-Al momento de generar la boleta, si se ingresó el mail, se enviará copia del mail al mismo.
<br>-En el caso que si se requiera generar trazabilidad con los clientes, es oblitario informar la información del cliente, en este caso el mismo rut del cliente será utilizado como identificador.
<br>-Si el cliente ya tiene correo en la ficha del sistema, no es necesario informar el mail en el envío de datos.
