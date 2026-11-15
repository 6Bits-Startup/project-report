# Conclusiones

## Conclusiones y recomendaciones.

### Conclusiones

1. El desarrollo de **OrganiK** permitió identificar una problemática real en la gestión de productos orgánicos: la fragmentación de información, el control manual de inventarios, la poca trazabilidad de lotes y la dependencia de canales informales como WhatsApp para coordinar pedidos entre minimarkets y proveedores.

2. Las entrevistas realizadas evidenciaron que tanto administradores de minimarkets como proveedores necesitan una solución centralizada, sencilla y accesible que les permita reducir errores operativos, anticipar vencimientos, controlar stock y mejorar la coordinación del abastecimiento.

3. La propuesta de **OrganiK** se diferencia de soluciones generales de inventario al enfocarse específicamente en productos orgánicos, integrando inventario, lotes, vencimientos, abastecimiento, proveedores y monitoreo de condiciones de conservación como temperatura y humedad.

4. La implementación de la landing page, publicada como sitio estático bilingüe con páginas legales y, desde el Sprint 3, con los videos About the Product y About the Team, permitió comunicar de manera clara la propuesta de valor del producto, sus funcionalidades principales, planes comerciales y canales de contacto.

5. La primera versión de la Web Application, desarrollada en Angular y organizada por bounded contexts y capas (domain, application, infrastructure, presentation), con internacionalización, permitió construir una base técnica ordenada que en el Sprint 3 se conectó a los Web Services sin rehacer las vistas, reemplazando solo la capa de infraestructura.

6. La primera versión de los Web Services (Sprint 3), construida con Spring Boot, Spring Data JPA, MySQL y autenticación JWT, con once bounded contexts y documentación OpenAPI publicada, hace posible el flujo central del Problem Statement: el minimarket solicita reposición, el proveedor responde con una orden de envío y, al aceptarla, los lotes se registran en el inventario y se genera una notificación. Esto da soporte técnico a los feature assumptions de abastecimiento y alertas; su validación con usuarios queda pendiente para el Sprint 4.

7. Asignar un bounded context del backend a cada integrante en el Sprint 3 distribuyó mejor el trabajo que en los sprints anteriores: todos los integrantes registraron commits en el repositorio de los Web Services. El trabajo colaborativo, apoyado en GitFlow, Conventional Commits, Discord y Jira, fortaleció la planificación y el seguimiento del proyecto.

### Recomendaciones

1. Realizar en el Sprint 4 las entrevistas de validación con administradores de minimarkets y proveedores sobre la versión desplegada, midiendo si los usuarios completan sin ayuda los flujos de registrar stock, atender una alerta de conservación y aceptar una orden de envío, y contrastar los resultados con los Hypothesis Statements.

2. Incorporar al menos un servicio externo de terceros en la solución (por ejemplo, envío de correos de notificación o consulta de datos climáticos para anticipar riesgos de conservación), tal como lo exige el alcance del proyecto.

3. Evitar la demora del primer acceso a los Web Services en el plan gratuito de Render (arranque en frío) antes de las sesiones de validación, y configurar el servidor de la especificación OpenAPI con la URL de producción para que la documentación permita probar los endpoints desplegados.

4. Mantener una interfaz responsive y simple, especialmente para dispositivos móviles, debido a que los usuarios gestionan muchas operaciones desde celular durante su jornada laboral.

5. Completar en la versión final de los videos About the Product y About the Team el testimonio de un usuario de las entrevistas de validación y el testimonio ante cámara de todos los integrantes.

## Video About-the-Team.

El video About the Team resume el proceso de trabajo del equipo **5Bits** durante el desarrollo de **OrganiK**. Inicia con escenas de las sesiones de trabajo del equipo en Discord, donde se planificó y revisó cada sprint, y con las estadísticas de colaboración en GitHub de la Web Application integrada con los Web Services. Luego presenta el testimonio ante cámara de los integrantes, quienes describen las actividades que realizaron, los outcomes logrados y las competencias que desarrollaron: la implementación de la Web Application, su integración con los Web Services y el despliegue; el desarrollo de los bounded contexts de conservación, comunicación y perfiles; y el desarrollo de los bounded contexts de proveedores y solicitudes de abastecimiento. Cierra con el mensaje de marca del producto.

Esta primera versión incluye los testimonios de tres integrantes. La versión final (TB2) incorporará el testimonio de todos los integrantes y una sección de retrospectiva del grupo.

![Video About the Team](./assets/chapter-05/s3-about-the-team.png)
*Figura: Cuadro del video About the Team.*

| Sección | Inicio (hh:mm:ss) |
| :--- | :--- |
| Apertura: OrganiK, About the Team | 00:00:00 |
| Nuestro proceso de trabajo (sesiones en Discord) | 00:00:05 |
| Colaboración en la Web Application (GitHub Insights) | 00:00:13 |
| Testimonios del equipo | 00:00:22 |
| Testimonio de Olivares Lao, Gustavo Alonso | 00:00:26 |
| Testimonio de Quispe Almonacid, Andre Sebastian | 00:01:18 |
| Testimonio de Torres Huaman, Alexis Calin | 00:02:28 |
| Cierre | 00:03:19 |

| Dato | Valor |
| :--- | :--- |
| Duración | 3:24 |
| YouTube (incrustado en la Landing Page) | https://www.youtube.com/watch?v=m9spOBsraMI |
| Microsoft Stream | [Ver video en Microsoft Stream](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202216448_upc_edu_pe/IQDozSp6DeUdTo11ckuUOs_VAcRhgh_q_IErDxqETbZubwk?e=jYkz7F) |
| Archivo | upc-pre-202620-1asi0729-7742-5Bits-about-the-team-sprint-3.mp4 |
