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

## leerob.com
| criterio | description |
|----------|---------|
| Tipología: | Estatico / No PWA |
| URL: | :https://leerob.com/ |
| Evidencias técnicas: | El sitio tienes archivos HTML, CSS y JS pre-renderizados. No realiza consultas a bases de datos en tiempo de ejecución ni genera contenido dinámico en el servidor. No tiene Service Workers configurados para funcionar offline como una PWA. |
| Comportamiento de navegación: | Navegación instantánea entre secciones. Al ser contenido estático, la estructura y los textos cargan de golpe sin saltos de contenido. |
| Tiempo de carga: | FCP: 0.3s y LCP: 0.5s (medido con PageSpeed Insights) |
| Interacción con servidor: | El servidor solo entrega los archivos físicos listos; no hay procesamiento backend ni intercambio de datos dinámicos. Si se desactiva JavaScript, el sitio sigue siendo 100% legible. |

# developer.mozilla.org
| criterio | description |
|----------|---------|
| Tipología: | Estatico |
| URL: | :https://developer.mozilla.org/ |
| Evidencias técnicas: | Las páginas de documentación se generan de forma estática a partir de archivos Markdown, Cuando cargada la aplicación, la navegación entre artículos se gestiona con React para no recargar el navegador. Cuenta con Service Workers (PWA parcial) para almacenar en caché las páginas visitadas. |
| Comportamiento de navegación: | Híbrido. La primera carga es estática y ultra rápida; las navegaciones internas son instantáneas a través del enrutamento del cliente. |
| Tiempo de carga: | FCP: 0.6s y LCP: 1.1s (medido con PageSpeed Insights) |
| Interacción con servidor: | El contenido principal es pre-renderizado desde una CDN. El servidor no procesa bases de datos para generar los artículos al momento de la petición. Si se desactiva JavaScript, el contenido de la documentación sigue siendo  legible gracias al HTML estático inicial. |
