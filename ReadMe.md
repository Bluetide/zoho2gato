#Zoho Fiscal
This applications retrieves invoices from Zoho and create independent JSON's for each invoice in the required input format for GatoMalo.

#Dependencies
This application is written in python3 3.4.1 and requires:

- Uses flask as the web server -
'sudo pip3 install flask'
- Requests
'sudo pip3 install requests'

# missing
- verificar las tasa de impuestos en translate_product(product)
- crear buscador para Proformas (asi no es necesario saberse el invoice id). escribir numero de proforma o cliente y mostrar lista de posibilidades.
- anular facturas.
- posiblemente incorporar capacidad de aplicar descuento por items, necesita desarrollo en gatomalo.
- enviar factura directo a gatomalo
- incorporar una pantalla para validar la informacion antes de imprimir.(bueno para debug y evitar errores).
- crear funcion para traer informacion del cliente
- tomar RUC del cliente e incorporarlo en el json para gatomalo
- tomar telefono del cliente incorporarlo en el json para gatomalo

#notas
- se utiliza el precio total de cada item para generar el json de gatomalo porque no hay forma de aplicar el descuento correctamente en gatomalo. Por eso se usa en cantidad siempre "1".
