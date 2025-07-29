Conjunto de datos de mensajería de DTDC
Un conjunto de datos reales de envíos de mensajería extraídos de las operaciones de DTDC en toda India. Este conjunto de datos captura el flujo completo de la logística de paquetes, incluyendo información del remitente/receptor, peso, modo de entrega, cargos y estado, lo que lo convierte en un recurso valioso para análisis, aprendizaje automático e investigación logística.

Descripción general del conjunto de datos
Cada fila representa un envío de mensajería reservado a través de DTDC, incluidos detalles como:

Lugar de recogida y entrega (ciudad, código postal, estado)
Peso del envío (real, volumétrico, facturable)
Modalidad de entrega y desglose de tarifas
Firmas, sellos de tiempo y detalles de GST (cuando corresponda)
Naturaleza del paquete: documentos o no documentos
Ejemplos de casos de uso
Optimización de rutas
Predicción del tiempo de entrega
Modelado de tarifas
Análisis de entregas de última milla
Mapas de calor geoespaciales de la demanda de mensajería


Esquema por columnas (descripciones)
Origen: La ciudad desde la que se reservó o envió originalmente el paquete.
Destino: La ciudad donde se pretende entregar el paquete.
Número de bolsa: un identificador interno único (a menudo UUID) que se utiliza para agrupar envíos en logística.
Fecha: La fecha en que se reservó el envío, representada en formato de número de serie de Excel.
Nombre del remitente: Nombre completo de la persona o empresa que envía el paquete.
Teléfono del remitente: Número de contacto móvil o fijo del remitente.
Dirección del remitente: Dirección completa del remitente para recogida y registros.
Ciudad del remitente: La ciudad del remitente puede duplicar el campo "Origen".
Estado del remitente: el estado de la India en el que se encuentra el remitente.
Código postal del remitente: el código postal de 6 dígitos de la ubicación del remitente.
GSTIN del remitente: Número de identificación GST del remitente (si corresponde para envíos comerciales).
Piezas totales: El número de paquetes físicos individuales incluidos en el envío.
Peso real: el peso físico real (en kilogramos) del(los) paquete(s).
Peso volumétrico: El peso calculado en función de las dimensiones del volumen, utilizado para fines de facturación.
Peso facturable: el peso utilizado para la facturación, normalmente el mayor entre el peso real o el peso volumétrico.
Trámites: Indica si se entregó el trámite junto con el paquete (Sí/No).
Firma del remitente: indica si el remitente firmó la documentación de envío (Sí/No).
Fecha del remitente: la fecha en la que el remitente completó la entrega o firmó los documentos, en formato de serie de Excel.
Nombre del destinatario: el nombre completo de la persona u organización que recibirá el paquete.
Teléfono del destinatario: el número de contacto del destinatario previsto.
Dirección del destinatario: La dirección de entrega completa donde debe enviarse el paquete.
Ciudad del destinatario: La ciudad del destinatario puede duplicar el campo “Destino”.
Estado receptor: el estado indio donde reside el destinatario.
Código postal del receptor: el código postal de 6 dígitos de la dirección de entrega.
Descripción: Una breve descripción textual del contenido del paquete (por ejemplo, documentos, artículos).
Servicios de Valor Agregado: Servicios opcionales añadidos al envío, como manejo de carga frágil, entrega express, seguro, etc.
Número de envío: el número de seguimiento oficial de DTDC asignado al envío.
Fecha de caducidad: Última fecha válida de entrega, tras la cual el envío puede caducar o ser devuelto. Se almacena como un número de serie de Excel.
Código de reserva: el código único que identifica la sucursal o el mostrador de reservas de DTDC.
Destinatario GSTIN: Número de identificación GST del destinatario (si corresponde).
Nombre del destinatario: un campo alternativo o duplicado para el nombre del destinatario.
Relación: describe la relación del receptor con el destinatario original (por ejemplo, usted mismo, personal, familia).
Sello de la empresa: Indica si se utilizó un sello de la empresa durante la recepción (Sí/No).
Firma del receptor: indica si el destinatario firmó la confirmación de entrega (Sí/No).
Fecha de recepción: la fecha en que se recibió el paquete, en formato de serie de Excel.
Tarifa: El cargo de envío base en rupias indias (₹).
Cargos VAS: Cargos adicionales por cualquier servicio de valor agregado aplicado al envío.
Importe total: el importe total facturado por el envío, incluida la tarifa y cualquier complemento.
Modo: El modo de envío elegido: superficie, aire o exprés.
Recargo por riesgo: indica quién asume la responsabilidad del riesgo: el propietario (remitente) o el transportista (DTDC).
Modo de pago: El método de pago utilizado al realizar la reserva, como efectivo, tarjeta, UPI, billetera, etc.
Naturaleza del envío: Indica el tipo de paquete: “Dox” para documentos o “No Dox” para bienes/mercancías.
Nota:
Tenga en cuenta que los ejemplos proporcionados son ficticios y tienen fines ilustrativos. Puede adaptar las descripciones y los ejemplos a las características específicas de su conjunto de datos. También puede contactarme por correo electrónico a: rrana157@gmail.com
