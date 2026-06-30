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

## Amazon.com
| criterio | description |
|----------|---------|
| Tipología: | Dinamico |
| URL: | :https://www.amazon.com/ |
| Evidencias técnicas: | 140 peticiones la mayoria amazon - PWA parcial: tiene un service worker activo(funcionalidad de caché/ sin pero no se ha detectado ningun archivo. |
| Comportamiento de navegación: | (MPA) multiplas paginas |
| Tiempo de carga: | FCP: 0.8s y LCP: 1.3s (medido con PageSpeed Insights) |
| Interacción con servidor: | Server-rendered: el element <body> contiene una cantidad significativa de contenido. Cuando JavaScript es desactivado el contenido permanece visible. |

## gabipanta.com
Interacción con servidor:
| criterio | description |
|----------|---------|
| Tipología: | Dinamico |
| URL: | :https://gabipanta.com/ |
| Evidencias técnicas: | Desarrollado con WordPress. Al hacer clic en las categorías o artículos, el navegador realiza una petición completa al servidor y recarga toda la página. No posee un Service Worker activo ni archivo de manifiesto entonces no es PWA. |
| Comportamiento de navegación: | (MPA) Multiples paginas con recarga completa del navegador en cada transición de sección. |
| Tiempo de carga: | FCP: 1.4s y LCP: 2.8s (medido con PageSpeed Insights) |
| Interacción con servidor: | Server-rendered (SSR): El servidor procesa el código PHP de WordPress, consulta la base de datos MySQL para traer los posts y genera el HTML final que se envía al usuario. Si se desactiva JavaScript, el contenido de los textos y las imágenes sigue visible. |
