# Cocina Paso a Paso

Prototipo de una app inclusiva para que estudiantes sigan la práctica de Cocina Internacional desde casa, con un adulto presente. Receta de trabajo: **Bruschetta de tomate**.

Proyecto escolar inspirado en el caso “Sabores sin barrera” (CBTis No. 92). Es una propuesta de diseño: no afirma haber demostrado mejoras en el aprendizaje. Los apoyos se ofrecen a todo el alumnado y no dependen de un diagnóstico.

## Cómo verlo

Es un solo archivo HTML sin dependencias ni instalación.

- **En tu computadora:** abre `index.html` en el navegador.
- **En línea con GitHub Pages:** en el repositorio ve a *Settings → Pages*, elige la rama `main` y la carpeta `/ (root)`, y guarda. En un minuto la app queda en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Qué incluye

| Módulo | Dónde verlo |
|---|---|
| Accesibilidad perfilable: Texto grande, Un paso a la vez y Escuchar, siempre visibles y guardados en el perfil | Barra superior y sección “Mis apoyos” |
| Navegación secuencial: un paso a la vez, casillas, contador “3 de 6” y cronómetro con pausa | Receta visual |
| Seguridad: checklist de higiene, alérgenos, organización y adulto presente; el botón sigue inactivo hasta confirmar los 4 puntos | “Antes de empezar” |
| Evidencias multiformato: foto, audio o texto breve | “Mi evidencia” |

Cambiar de apoyo a mitad de la receta no borra el progreso. Ningún apoyo se salta el checklist de seguridad.

## Abrir una pantalla directamente

Agrega parámetros a la URL, por ejemplo:

```
index.html?pantalla=receta&paso=3&unpaso=1&texto=grande
```

Pantallas: `inicio`, `catalogo`, `apoyos`, `receta_info`, `seguridad`, `receta`, `reto`, `evidencia`, `cierre`, `adulto`, `proyecto`.

## Voz con audios pregrabados

El botón "Escuchar" reproduce los audios de voz IA de la carpeta `audio/` (15 MP3, uno por texto). Si falta alguno, usa la voz del dispositivo con el estilo elegido en "Mis apoyos" (Natural, Asistente IA o Tranquila). La lista de textos y nombres de archivo está en `audio/Guion_de_voz.md` y `audio/Guion_de_voz.csv` (15 audios).

Nota: los audios se escuchan al publicar el sitio (GitHub Pages) o al abrirlo con un servidor local. Algunos navegadores bloquean audios locales si abres `index.html` con doble clic.

## Datos y privacidad

El prototipo guarda el perfil y el progreso solo en el navegador (`localStorage`). Las fotos y los audios no se suben a ningún servidor. El botón “Borrar mis datos de prueba” (sección “El proyecto”) limpia todo.

## Estructura

```
index.html   Prototipo (HTML, CSS y JavaScript en un solo archivo)
docs/        Análisis UX (PDF), pantallas (PDF) y arquitectura de datos (PDF y PNG)
capturas/    Capturas de las 12 pantallas
audio/       15 audios MP3 de la voz IA y su guion
```

## Uso de IA

El primer borrador del prototipo, del análisis y del modelo de datos se hizo con apoyo de un asistente de IA (Claude). El equipo revisó y ajustó las decisiones de diseño.
