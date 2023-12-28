Suppliers User stories

* Como usuario Crear cuenta de usuario para proveedor
    - enviar *notificacion* a proveedor sobre su nueva cuenta
      - el correo contendra un link hacia la plataforma
    > Indicar el nombre del grupo que podra crear la cuenta proveedor

    > El rol supplier sera creado para los proveedores


* Como proveedor nuevo deseo ingresar mis datos en la plataforma


  * Credenciales
    - Las credenciales provistas son de la cuenta del contacto del proveedor
    - El proveedor debera ingresar en la plataforma forma mediante un link en la notificacion
    - El proveedor debera ingresar las credenciales provistas en el correo
    - La plataforma obliga a cambiar la contrasenia al momento de ingresar las credenciales correctas


  * Formulario de registro (formulario se basara en la imagen de proveedor enviado por FA)
    - El proveedor debera ingresar al formulario de auto registro (portal de proveedor -> record producer)
    - El formulario debera validar la informacion provista en los tres campos segun los documentos ingresados como attachment
    - El formulario tendra un contacto prellenado con la info del usuario creado anteriormente;
    - > *Se debera considerar la solicitud de nuevos contactos en una sig version, por ahora el registro y asociacion de contacto estara a cargo de un usuario de FA*

    **Validaciones**
    - Validar que se ingresaron los RFC y datos requeridos en el formulario
    - Validar datos de indetificacion de proveedor (Solicitar: Termino manejado por FA)
      > por ahora el identificador se ingresara manualmente por el proveedor en tres campos dentro el formulario


  * Envio de datos
    - Al presionar en el boton Guardar o Enviar el formulario guardara los datos ingresados con previa validacion de los datos
    - Al guardar el registro en la tabla, se enviara una *notificacion* al o encargados del registro de proveedores para que validen la informacion
    - > Validar la informacion del proveedor contra SAT podra ser contemplada en una siguiente version


  * Validacion de datos por encargado de registro de proveedores
    - Al recibir una notificacion de proveedor registrado, el encargado podra abrir el formulario del proveedor y validar la informacion para consolidar la informacion en el sistema y "activar" al proveedor
    - > Podria enviarse notificacion al proveedor para indicarle que se activo sus "datos" en la plataforma


  * Integracion de datos
    - Una vez validados los datos del proveedor por el encargado de FA, se realizara la integracion de estos datos con servicios de FA
    - **Se debera hacer match de indentificadores de servicios de FA y Servicenow**
    - Despues de hacer el match entre identificadores y ambos servicios se actualizara la informacion en ServiceNow para integraciones de Ordenes de compra, relacion con productos-proveedor, etc.


  * Ingreso a plataforma del proveedor
    - > El proveedor podra acceder a la plataforma una vez que sus datos fueran validados y "activados", Vale decir que podra ver sus casos y todos las opciones de proveedor, mientras no esten validados solo debera ver el formulario de registro con el estado respectivo.


  * Contactos de Proveedor
    - Registrar informacion de contactos
    - Cada proveedore debera tener dos contactos: Transportista y Ventas
      > Los transportistas o quien entrega deberia tener acceso a la plataforma?



------------------------------------------------------------------

Oredenes de compra

