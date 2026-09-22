# Portfolio — Game Programmer

Template estático (HTML + CSS + JS, sin frameworks) inspirado en el editor de un motor de juegos:
un panel de **Hierarchy** a la izquierda (tu navegación) y paneles de **Inspector** a la derecha
(cada sección de tu CV como si fuera un componente/script).

## Archivos

```
game-dev-portfolio/
├── index.html   → contenido y estructura
├── style.css    → toda la identidad visual (paleta, tipografía, layout)
├── script.js    → navegación activa, menú mobile, botones decorativos
└── assets/      → poné acá tu foto y capturas/gifs de proyectos
```

## Cómo personalizarlo

1. **Reemplazá los textos placeholder** en `index.html`: nombre, rol, bio, experiencia,
   proyectos, educación, logros, skills e intereses. Todo está en inglés porque es la
   convención para portfolios que vas a compartir en LinkedIn/GitHub, pero podés traducirlo.
2. **Tu foto**: reemplazá el `<svg>` placeholder dentro de `.hierarchy__avatar` y `.about__photo`
   por un `<img src="assets/photo.jpg" alt="Your Name">`.
3. **Barras de Skills**: cada barra usa `style="--fill:XX%"` — cambiá el número (0–100) y el
   texto del `<span class="stat-bar__value">`.
4. **Demo reel / video**: el recuadro punteado en "About" es un placeholder. Podés pegar ahí
   un `<iframe>` de YouTube o un `<video>`.
5. **Links**: actualizá `href` de LinkedIn, GitHub y email en el `<footer>` del hierarchy panel,
   y los links de "Play"/"Repo" en cada tarjeta de proyecto.

## Cómo publicarlo gratis en GitHub Pages

1. Creá un repositorio en GitHub llamado exactamente `tu-usuario.github.io`
   (reemplazando `tu-usuario` por tu nombre de usuario de GitHub).
2. Subí estos tres archivos (`index.html`, `style.css`, `script.js`) y la carpeta `assets/`
   a la raíz de ese repositorio.
3. Andá a **Settings → Pages** del repo y confirmá que la fuente sea la rama `main` (carpeta `/root`).
4. En unos minutos tu portfolio va a estar online en `https://tu-usuario.github.io`.

Si preferís no usar el nombre especial del repo, también podés crear un repo con cualquier
nombre y activar Pages igual — en ese caso la URL va a ser `https://tu-usuario.github.io/nombre-del-repo`.

## Notas técnicas

- Sin dependencias ni build step: abrí `index.html` directo en el navegador para probarlo local.
- Tipografías: Space Grotesk (títulos), Inter (texto), JetBrains Mono (detalles tipo código) —
  cargadas desde Google Fonts.
- Responsive: en pantallas chicas el panel de Hierarchy se convierte en un drawer (☰ arriba a la izquierda).
- Respeta `prefers-reduced-motion` y tiene estados de foco visibles para navegación por teclado.
