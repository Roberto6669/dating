# Vibra — Sitio web de citas

Sitio web de citas estilo landing moderna (inspirado en tinder.com), con paleta azul → turquesa. Ancho completo, no es un marco de teléfono. Construido en React (pre-compilado, sin Babel) pensando en la futura app móvil.

## Cómo abrirlo

Doble clic en `index.html` (cualquier navegador). Necesita internet para cargar React y las fotos de ejemplo.

## Qué incluye

Una sola página con dos grandes vistas:

**1. Landing (página de inicio)**
- Barra de navegación fija con logo, menú e botones *Iniciar sesión* / *Crear cuenta*.
- Hero a pantalla completa con degradado azul-turquesa, titular y tarjetas de perfil.
- Sección "Cómo funciona" (3 pasos).
- Sección "Por qué Vibra" (4 funciones).
- "Historias Vibra" (testimonios con foto).
- Banda de llamada a la acción + footer completo.

**2. Login / Registro**
- Modal con pestañas Iniciar sesión / Registrarse (simulado). Cualquier dato lleva a Explorar.

**3. Explorar (la app dentro del website)**
- Layout web de ancho completo: panel de filtros a la izquierda + tarjeta de perfil grande a la derecha.
- Filtros: género, edad, distancia, intención e intereses.
- Botones Pasar / Super like / Me gusta.
- Pestaña de Matches con cuadrícula.
- Popup "¡Es un match!".

## Marca

- Nombre: **Vibra**
- Colores: degradado azul `#1b66ff` → turquesa `#10d6c2`

## Datos

Los perfiles de ejemplo están en el array `PROFILES` dentro de `index.html`. Fotos de randomuser.me y Unsplash (demo).

## Publicar (GitHub + Render)

1. Guarda cambios y sube a GitHub:
   ```bash
   git add -A && git commit -m "rediseño: sitio web Vibra" && git push
   ```
2. En Render (Static Site) el sitio se redespliega solo. Build Command vacío, Publish Directory `.`.

## Próximos pasos hacia la app móvil

Backend real (login + perfiles + matches guardados), chat, geolocalización, y migración a React Native reutilizando estos componentes.
