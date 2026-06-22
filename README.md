# Spark — Prototipo de Dating

Prototipo navegable de una app de citas estilo **Tinder + Match** (swipe + filtros), construido en React. Diseñado mobile-first pensando en la futura app para celular.

## Cómo abrirlo

Haz doble clic en `index.html` (se abre en cualquier navegador). No requiere instalación. Necesita internet para cargar React y las fotos de ejemplo.

> Tip: en Chrome/Safari activa la vista móvil (F12 → ícono de celular) para verlo como en un teléfono.

## Qué incluye

- **Swipe de cartas**: arrastra con el mouse/dedo a la derecha (LIKE) o izquierda (NOPE), con sellos animados.
- **Botones de acción**: deshacer, nope, super like (★), me gusta (♥), boost.
- **Filtros de búsqueda**: género, rango de edad, distancia, intención (serio/casual/conocer gente) e intereses.
- **Pantalla de matches/likes**: cuadrícula con las personas a las que diste like, marca de "nuevo" y "super".
- **Popup "¡Es un match!"**: aparece cuando hay match mutuo (simulado).
- **Navegación inferior**: descubrir, filtros, matches.

## Referencias de diseño (investigación)

- **Tinder** — mecánica de swipe, volumen de perfiles, foto primero. ~75M usuarios/mes.
- **Hinge** — perfiles con prompts e intereses, enfoque en relaciones serias.
- **Bumble** — la mujer escribe primero, modos BFF/Bizz.
- **Match.com** — búsqueda con filtros detallados, relaciones serias.

## Datos

Los 12 perfiles de ejemplo están en el array `PROFILES` dentro de `index.html`. Edita ahí para cambiar nombres, fotos, intereses, etc. Las fotos vienen de randomuser.me (demo).

## Próximos pasos hacia la app móvil

1. **Backend / base de datos** — registro, login, perfiles reales, fotos subidas (ej. Supabase o Firebase).
2. **Algoritmo de matching** — guardar likes y detectar matches mutuos reales (no simulados).
3. **Chat** — mensajería entre matches.
4. **Geolocalización** — distancia real basada en GPS.
5. **Migrar a React Native** — el código ya está en componentes React, lo que facilita el port a app iOS/Android.
6. **Moderación y seguridad** — verificación de fotos, reportes, bloqueo.

## Estructura del código (`index.html`, un solo archivo)

- `App` — estado global, filtros y tabs.
- `Deck` / `SwipeCard` — la pila de cartas y la lógica de arrastre.
- `Actions` — botones inferiores.
- `Filters` — panel de filtros.
- `Matches` — cuadrícula de likes.
- `MatchPopup` — modal de match.
