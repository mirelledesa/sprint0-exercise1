# sprint0-exercise1
Application analysis

## Twitter.com
| criterio | description |
|----------|---------|
| Tipología: | Dinamico  |
| URL: | :https://x.com/ |
| Evidencias técnicas: | Cuando la aplicacion carga, la navegacion por el menu no recarga la pestaña del navegador. Si se desactiva JavaScript, el sitio no funciona. Es una PWA completa|
| Comportamiento de navegación: | (SPA) Navegacion instantanea por el cliente, el feed se actualiza constantemente sin interrumpir la experiencia del usuario. |
| Tiempo de carga: | FCP: 1.1s y LCP: 2.1s (medido con PageSpeed Insights) |
| Interacción con servidor: | Dependencia absoluta de una API. Intercambio constante de datos para mostrar novos tweets o interacciones en tiempo real. |

## Airbnb.com
| criterio | description |
|----------|---------|
| Tipología: | Dinamico / SPA parcial |
| URL: | :https://www.airbnb.com/ |
| Evidencias técnicas: | Carga inicial del servidor (SSR). Registra Service Workers para optimizar la caché de imágenes y recursos, PWA parcial . |
| Comportamiento de navegación: | (SPA / Hibrido) Transiciones suaves entre paginas |
| Tiempo de carga: | FCP: 0.9s y LCP: 1.8s (medido con PageSpeed Insights) |
| Interacción con servidor: | Carga datos dinamicamente en segundo plano a traves de peticiones a medida que el usuario interactua con el mapa y los filtros. |


URL:https://x.com/
Evidencias técnicas: Actualizacion en tempo real - Interaccion fluida -
