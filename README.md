# ApiErp
Integración de Aplicaciones Externas con ERP Factronica

ApiERP permite que aplicaciones externas puedan comunicarse con el Sistema ERP FacTronica.
<br>La comunicación es Bi-Direccional, lo que siginifica que permite tanto recibir como enviar datos. 
<br>El formato establecido para el intercambio de datos es a través de objetos JSON
<br>
<br>A continuación se detallan los módulos que Actualmente permiten Integración con Aplicaciones externas.
<br>Para cada Módulo a integrar se aplica un Grupo de Variables predefinidas.
<br>
<br><b>MÓDULOS:</b>
<br>-Clientes
<br>-Proveedores
<br>-Trabajadores
<br>-Facturas de Venta
<br>-Boletas de Venta (<a href="https://github.com/FacTronica/ApiErp/blob/master/ApiBoletaVenta">Ver Documentación</a>)
<br>-Notas de Venta
<br>
<br><b>NOTAS:</b>
<br>-Por motivos de seguridad, las URL's de la API no son publicadas y se envian al cliente vía email, luego de haber contratado los servicios de Factronica SpA.
<br>-A cada cliente se le asigna una llave de seguridad (TOKEN) la cual debe ser enviada en el JSON para así poder tener acceso a la API.
