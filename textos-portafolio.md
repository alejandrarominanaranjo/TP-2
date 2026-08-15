# Textos para el Portafolio de Proyectos — TP2

> Instrucciones: copiá cada bloque dentro de la ficha correspondiente en Canva o
> Google Docs. Los textos entre [corchetes] son los únicos que tenés que
> revisar o completar con tu criterio (fechas reales, capturas, link del repo).

---

## 1. Landing page — "Cumbre Libre"

### Historia de usuario / el gran problema
Como usuaria interesada en hacer trekking en Mendoza, necesito encontrar
rápido información clara sobre las rutas disponibles (distancia, dificultad,
duración) y poder reservar una excursión sin tener que llamar por teléfono,
incluso estando en el celular. El problema a resolver fue diseñar una página
de aterrizaje (landing page) que comunique la propuesta de una agencia de
trekking en pocos segundos y facilite el contacto, adaptada a cualquier
tamaño de pantalla.

### Por qué se eligieron estas tecnologías
Se utilizó **HTML5** semántico para estructurar el contenido (`header`,
`nav`, `section`, `footer`) y **Bootstrap 5** porque su sistema de grillas y
componentes (navbar responsive, carrusel y modal) permiten cumplir con los
requisitos de la consigna —menú hamburguesa, carrusel navegable y cuadro
modal— sin tener que programar esas interacciones desde cero en JavaScript,
priorizando el tiempo de desarrollo en la identidad visual del sitio. El CSS
propio (`style.css`) se separó del framework para mantener ordenada la
paleta de colores y la tipografía particular del proyecto.

### Rol de cada integrante
Equipo de un solo integrante. Cumplí los cuatro roles:
- **Analista:** definí el problema del usuario y el objetivo de la página.
- **Diseñadora:** elegí la paleta, tipografía y el layout de cada sección.
- **Programadora:** maqueté el HTML, el CSS y configuré los componentes de Bootstrap.
- **Documentadora:** redacté esta ficha y subí el proyecto a GitHub.

### Bitácora de colaboración
| Fecha | Actividad |
|---|---|
| [dd/mm] | Investigación de rutas de trekking en Mendoza y definición de la temática. |
| [dd/mm] | Boceto de la estructura de secciones (hero, rutas, features, footer). |
| [dd/mm] | Maquetado del HTML con Bootstrap (navbar, carrusel, modal). |
| [dd/mm] | Escritura del CSS propio (paleta, tipografía, responsive). |
| [dd/mm] | Pruebas en celular y ajustes de responsive. Subida a GitHub. |

### Reflexión / resultados
El mayor desafío fue lograr que el carrusel y el modal se vieran coherentes
con la paleta elegida, ya que Bootstrap trae sus propios estilos por
defecto. Resolverlo reforzó cómo funciona la especificidad en CSS al
sobrescribir clases del framework. Como resultado, la página es
responsive: probada en un viewport de 375px de ancho (celular estándar),
el menú colapsa correctamente a hamburguesa y el carrusel se reduce de
altura sin recortar contenido.

### Captura y enlace
- [Insertar acá la captura más representativa de la landing]
- Repositorio: [https://github.com/tu-usuario/tu-repo]

---

## 2. Formulario — "Refugio del Cóndor"

### Historia de usuario / el gran problema
Como comensal que quiere reservar una mesa en un restaurante de montaña,
necesito completar un formulario simple desde mi celular y recibir
confirmación de que mis datos se cargaron bien, sin poder enviar el
formulario si me olvidé un dato obligatorio (por ejemplo, el teléfono o la
fecha). El problema a resolver fue construir un formulario de reserva con
validación clara antes del envío.

### Por qué se eligieron estas tecnologías
Se usó **HTML5** con atributos nativos de validación (`required`,
`pattern`, `type="email"`, `type="date"`, `type="number"` con `min`/`max`)
porque el navegador ya resuelve gran parte de la validación sin
JavaScript adicional. Se combinó con las clases de validación de
**Bootstrap** (`needs-validation`, `is-invalid`, `was-validated`) para
mostrar mensajes de error prolijos y consistentes con el resto del sitio,
y un mínimo de JavaScript solo para simular el envío y mostrar el mensaje
de confirmación.

### Rol de cada integrante
Equipo de un solo integrante. Cumplí los cuatro roles:
- **Analista:** definí qué datos eran obligatorios y por qué.
- **Diseñadora:** elegí la paleta (madera, verde bosque) acorde a la temática.
- **Programadora:** implementé la validación HTML5 y el script de envío simulado.
- **Documentadora:** redacté esta ficha y subí el proyecto a GitHub.

### Bitácora de colaboración
| Fecha | Actividad |
|---|---|
| [dd/mm] | Definición de la temática y de los campos del formulario. |
| [dd/mm] | Maquetado del formulario con Bootstrap. |
| [dd/mm] | Configuración de validaciones HTML5 (pattern, required, min/max). |
| [dd/mm] | Script de validación y mensaje de éxito al enviar. |
| [dd/mm] | Pruebas de casos inválidos (campos vacíos, teléfono con letras). Subida a GitHub. |

### Reflexión / resultados
Probar el formulario con datos incorrectos a propósito (dejar el teléfono
vacío, poner letras en vez de números) ayudó a verificar que cada mensaje
de error apareciera en el campo correcto. El resultado es un formulario
que no permite el envío hasta que los 7 campos obligatorios son válidos,
y que confirma visualmente el éxito del envío sin recargar la página.

### Captura y enlace
- [Insertar acá la captura del formulario, idealmente mostrando un error de validación]
- Repositorio: [https://github.com/tu-usuario/tu-repo]

---

## 3. Guía de estilo — "Casa Terracota"

### Historia de usuario / el gran problema
Como diseñadora que arma la identidad visual de una marca de cerámica
artesanal, necesito un documento de referencia (guía de estilo) que
muestre en un solo lugar la paleta de colores, la tipografía y los
componentes reutilizables (botones, enlaces, acordeón) para que cualquier
pieza nueva del sitio mantenga la misma coherencia visual.

### Por qué se eligieron estas tecnologías
La consigna pedía **HTML5 y CSS puro**, sin framework, así que se aprovechó
para practicar CSS "a mano": el acordeón se resolvió con las etiquetas
nativas `<details>` y `<summary>` (sin una sola línea de JavaScript), el
efecto de botón 3D se logró con una sombra sólida que se "hunde" al hacer
clic (`:active` + `transform`), y los enlaces animados usan una transición
de `background-size` sobre un degradado en vez de un `border-bottom` fijo,
para que la línea de color crezca de forma animada al pasar el mouse.

### Rol de cada integrante
Equipo de un solo integrante. Cumplí los cuatro roles:
- **Analista:** definí qué componentes debía mostrar la guía según la consigna.
- **Diseñadora:** elegí la paleta terracota/oliva y la tipografía Fraunces + Inter.
- **Programadora:** programé cada componente en CSS puro (acordeón, botones, enlaces, foco).
- **Documentadora:** redacté esta ficha y subí el proyecto a GitHub.

### Bitácora de colaboración
| Fecha | Actividad |
|---|---|
| [dd/mm] | Definición de la temática (marca de cerámica) y de la paleta de colores. |
| [dd/mm] | Programación del acordeón con `<details>`/`<summary>`. |
| [dd/mm] | Programación de los botones 3D y los enlaces animados. |
| [dd/mm] | Ajuste del borde de foco en el campo de formulario de muestra. |
| [dd/mm] | Revisión general de contraste y prolijidad del código. Subida a GitHub. |

### Reflexión / resultados
Lograr el acordeón sin JavaScript fue el punto más interesante: usar
`<details>` es una solución 100% de HTML5, accesible por teclado por
defecto, y más liviana que depender de un script. El resultado es una guía
que funciona igual de bien sin conexión a internet salvo por las fuentes
de Google Fonts, ya que no depende de ningún framework externo.

### Captura y enlace
- [Insertar acá la captura de la guía de estilo, mostrando el acordeón abierto]
- Repositorio: [https://github.com/tu-usuario/tu-repo]
