## DIU - Practica2, entregables

### Ideación 
* Malla receptora de información

  [Feedback Grid Template (Copy).pdf](https://github.com/user-attachments/files/19999651/Feedback.Grid.Template.Copy.pdf)
  ![image](https://github.com/user-attachments/assets/19934bed-a90d-4673-b79a-0d5efc80cbef)


* Mapa de empatía

  
[Empathy Map (Copy).pdf](https://github.com/user-attachments/files/19999653/Empathy.Map.Copy.pdf)
![image](https://github.com/user-attachments/assets/45ebd964-5fab-4126-ad7f-4d94f3f3f1ee)


  
* Point of View 


### PROPUESTA DE VALOR
* ScopeCanvas

  [Scope Canvas (Community) (Copy).pdf](https://github.com/user-attachments/files/19999640/Scope.Canvas.Community.Copy.pdf)
  ![image](https://github.com/user-attachments/assets/b4f9612e-d355-49bf-864f-4a32ca2c73ab)



### TASK ANALYSIS

* User Task Matrix
  
| Acción | Productores | Compradores | Empleados | Media |
|:------------------------------------------------------------------------------------------------|:-----------:|:-----------:|:---------:|:-----:|
| Filtrar productos por temporada y origen según disponibilidad local | 1 | 5 | 3 | 3.00 |
| Personalizar cestas con tus preferencias dietéticas y de sabor | 1 | 5 | 2 | 2.67 |
| Activar suscripción semanal o mensual ajustando día y hora | 0 | 5 | 4 | 3.00 |
| Puntuar y reseñar cada producto con fotos y comentarios | 0 | 5 | 1 | 2.00 |
| Guardar favoritos para futuros pedidos y compararlos fácilmente | 0 | 5 | 1 | 2.00 |
| Completar la compra en tres clics sin formularios complejos | 0 | 5 | 4 | 3.00 |
| Compartir recetas con la comunidad y consejos de cocina | 0 | 4 | 2 | 2.00 |
| Apuntarse a talleres de cocina sostenible presenciales y online | 1 | 4 | 3 | 2.67 |
| Devolver envases reutilizables para obtener descuentos extra | 0 | 4 | 3 | 2.33 |
| Invitar amigos para ganar créditos y descuentos exclusivos | 0 | 4 | 2 | 2.00 |
| Registrar productos con información de origen y certificaciones | 5 | 1 | 3 | 3.00 |
| Actualizar stock y cantidades en tiempo real | 5 | 1 | 4 | 3.33 |
| Ver y gestionar pedidos recibidos | 5 | 2 | 4 | 3.67 |
| Comunicar plazos de cosecha y entrega | 5 | 3 | 3 | 3.67 |
| Recibir y revisar feedback de clientes | 5 | 1 | 3 | 3.00 |
| Gestionar devoluciones y coordinar recogidas | 4 | 2 | 4 | 3.33 |
| Atender consultas y soporte al cliente en tiempo real | 1 | 4 | 5 | 3.33 |
| Procesar pedidos para envío | 1 | 1 | 5 | 2.33 |
| Gestionar planes de suscripción de clientes | 1 | 3 | 5 | 3.00 |
| Modera y aprueba contenido en la comunidad | 1 | 2 | 5 | 2.67 |
| Organizar y coordinar talleres y eventos | 2 | 3 | 5 | 3.33 |
| Generar informes de impacto (CO₂ evitado, estadísticas) | 3 | 1 | 5 | 3.00 |
| Añadir productos al carrito | 0 | 5 | 2 | 2.33 |
| Eliminar productos del carrito | 0 | 5 | 2 | 2.33 |
| Completar el checkout paso a paso | 0 | 5 | 4 | 3.00 |
| Registrar nueva cuenta de usuario | 0 | 4 | 3 | 2.33 |
| Iniciar sesión para acceder a funcionalidades avanzadas | 0 | 4 | 3 | 2.33 |
| Consultar la sección de Preguntas Frecuentes (FAQs) | 1 | 4 | 3 | 2.67 |
| Contactar soporte vía chat, email o formulario | 1 | 4 | 4 | 3.00 |
| Monitorizar stock y recibir notificaciones de disponibilidad | 5 | 2 | 4 | 3.67 |
 
* User/Task flow


### ARQUITECTURA DE INFORMACIÓN

* Sitemap
  
![sitemap](https://github.com/user-attachments/assets/722a766b-e7b2-4fa9-9b37-4ef1fb07363b)

* Labelling 

| Ruta | Etiqueta | Definición |
|----------------------------------------------- |----------------------------------|---------------------------------------------------------------------------|
| `/carrito` | Carrito | Vista principal con todos los productos seleccionados. |
| `/checkout` | Realizar pedido | Flujo de finalización de la compra. |
| `/checkout/entrega` | Método de entrega | Selección de modalidad y horario de envío. |
| `/checkout/pago` | Método de pago | Elección del sistema de pago y datos de facturación. |
| `/checkout/cupon` | Introducir cupón | Aplicación de un código descuento al pedido. |
| `/tienda/buscar` | Buscador | Búsqueda de productos por nombre o palabra clave. |
| `/tienda/filtrar` | Filtrar productos | Filtros de categoría, precio y temporada para el catálogo. |
| `/tienda/ordenar` | Ordenar productos | Opciones para reordenar la lista (precio, popularidad, novedades). |
| `/admin/productos/{id}/editar` | Editar producto | Modificar datos e imágenes de un producto desde el panel interno. |
| `/admin/productos/{id}/publicar` | Ocultar/mostrar | Activar o desactivar la visibilidad de un producto en la tienda. |
| `/producto/{id}` | Ver ficha técnica | Detalle completo del producto: descripción, certificaciones e imágenes. |
| `/producto/{id}/reseñar` | Reseñar producto | Formulario para valorar y comentar sobre un producto. |
| `/register` | Registrar | Formulario de alta para nuevos usuarios. |
| `/login` | Iniciar sesión | Área de acceso con email y contraseña. |
| `/password-reset` | Olvidé contraseña | Proceso de recuperación de la contraseña vía email. |
| `/login/remember` | Recordarme | Opción para mantener la sesión iniciada en el dispositivo. |
| `/actividades` | Listar actividades | Catálogo de cursos y talleres disponibles (presencial y online). |
| `/actividades/favoritos` | Añadir a favoritos (actividad) | Guardar una actividad en la lista personal de favoritos. |
| `/actividades/{id}` | Mostrar información (actividad) | Detalle completo de la actividad: temario, fechas y requisitos. |
| `/actividades/{id}/share` | Compartir actividad | Compartir enlace de la actividad en redes sociales. |
| `/actividades/{id}/inscribir` | Inscribirse a actividad | Registro en el curso o taller seleccionado. |
| `/actividades/{id}/temario` | Mostrar temario | Consulta del programa y contenidos de la actividad. |
| `/actividades/{id}/solicitudes` | Ver solicitudes | Gestión de matrículas pendientes de aprobación. |
| `/admin/actividades/{id}` | Gestionar curso | Panel interno para confirmar plazas y coordinar la formación. |
| `/promociones` | Promociones activas | Listado de ofertas y descuentos disponibles. |
| `/admin/promociones/nueva` | Añadir promoción | Formulario para crear nuevas promociones y packs. |
| `/sobre-nosotros` | Sobre nosotros | Sección corporativa con misión, visión, valores y RSC. |
| `/sobre-nosotros/historia` | Historia | Línea de tiempo y principales hitos de la organización. |
| `/sobre-nosotros/contacto` | Contacto | Formulario y datos de ubicación y atención al cliente. |
| `/sobre-nosotros/faqs` | FAQs | Preguntas frecuentes institucionales. |
| `/admin/ventas` | Listar ventas | Panel de visualización de todas las ventas registradas. |
| `/admin/ventas/devoluciones` | Gestionar devoluciones | Área para tramitar devoluciones y coordinar recogidas. |
| `/admin/ventas/stock` | Gestionar stock | Herramienta para ajustar y controlar el inventario de productos. |
| `/terminos` | Términos y Condiciones | Enlace principal a todas las políticas y condiciones de uso. |
| `/terminos/aviso-legal` | Aviso Legal | Información legal obligatoria de la empresa. |
| `/terminos/politica-privacidad` | Política de Privacidad | Detalles de cómo se recogen, usan y protegen los datos personales. |
| `/terminos/politica-cookies` | Política de Cookies | Descripción del uso de cookies y opciones para configurarlas. |
| `/terminos/politica-envios` | Política de Envíos | Condiciones y costes asociados a la entrega de los pedidos. |
| `/terminos/faqs-general` | FAQ General | Respuestas a las dudas más habituales sobre la plataforma. |
| `/contacto` | Contacto y Redes Sociales | Página de contacto y enlaces a los perfiles oficiales en redes sociales. |
| `/contacto/formulario` | Formulario de Contacto | Envío de consultas directas al equipo de atención al cliente. |
| `mailto:soporte@valleyvega.org` | Correo electrónico | Dirección de email para soporte y atención de incidencias. |
| `/contacto/chat` | Chat en línea | Acceso a soporte en tiempo real a través de chat. |
| `/contacto/redes` | Redes sociales | Enlaces a perfiles en Instagram, Facebook, Twitter, etc. |

###  Wireframe 

https://www.figma.com/design/4o4orsnCKKGm57zFW5iFfR/GreenBasket---Homepage?m=auto&t=pKPH3UWCigMaxJjF-6
![GreenBasket - Homepage-1](https://github.com/user-attachments/assets/2db375d9-bbfc-42ed-8510-4e076eecf005)


### Conclusiones  
(incluye valoración de esta etapa)


>>>> Este fichero se debe editar para que cada evidencia quede enlazada con el recurso subido a la carpeta de la practica. Se pide más detalle técnico en las descripciones de lo que sería el README principal del repositorio y que corresponde a la descripcion del Case Study.
>>>> Termine con la seccion de Conclusiones para aportar una valoración final del equipo sobre la propia realización de la práctica
