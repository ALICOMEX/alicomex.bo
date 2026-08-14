# ALICOMEX — sitio web estático

Proyecto listo para publicarse en GitHub Pages, Netlify, Cloudflare Pages o cualquier hosting estático. No requiere Node.js, paquetes ni compilación.

## Archivos principales

- `index.html`: contenido y metadatos del sitio.
- `styles.css`: diseño completo y adaptación para celulares, tablets y computadoras.
- `script.js`: carrusel automático de 14 segundos, controles, teclado, preguntas frecuentes y panel de cotización.
- `assets/`: logo e imágenes del sitio.

## Publicar con GitHub Pages

1. Crea un repositorio nuevo en GitHub.
2. Sube **todo el contenido de esta carpeta** a la rama `main`.
3. En GitHub abre `Settings` → `Pages`.
4. En `Build and deployment`, elige `Deploy from a branch`.
5. Selecciona la rama `main`, la carpeta `/ (root)` y guarda.

GitHub mostrará la dirección pública cuando termine la publicación.

## Vista local

Puedes abrir `index.html` directamente. Para una prueba más fiel, usa un servidor local, por ejemplo:

```bash
python3 -m http.server 8080
```

Después visita `http://localhost:8080`.

## Formulario de cotización

GitHub Pages no procesa formularios por sí solo. El panel funciona visualmente y valida los campos, pero para recibir solicitudes debes conectarlo a tu WhatsApp, correo o a un servicio de formularios. La lógica está al final de `script.js`, en el evento `submit` de `#quote-form`.
