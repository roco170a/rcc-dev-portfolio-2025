# 📄 README.md — Proyecto Jekyll con Tema Minimal Mistakes

> ✅ **Para principiantes en Ruby, Jekyll y Minimal Mistakes**  
> 🌐 Sitio web personal, blog o portafolio estático  
> 🎨 Diseño limpio, responsive y altamente personalizable

---

## 🧭 ¿Qué es esto?

Este proyecto es un sitio web estático construido con **[Jekyll](https://jekyllrb.com/)**, un generador de sitios estáticos muy popular, usando el tema **[Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)**, conocido por su diseño limpio, profesional y fácil de personalizar.

**No necesitas ser experto en programación** para usarlo. Solo necesitas seguir los pasos de este README.

---

## 🧰 Requisitos previos

Antes de empezar, asegúrate de tener instalado en tu computadora:

### 1. **Git**  
Para clonar el repositorio y manejar versiones.  
👉 [Descargar Git](https://git-scm.com/)

### 2. **Ruby** (versión 2.5 o superior)  
Jekyll está hecho en Ruby.  
👉 [Instalar Ruby en Windows, macOS o Linux](https://www.ruby-lang.org/es/documentation/installation/)

> 💡 En macOS, Ruby suele venir preinstalado. En Windows, te recomendamos usar [RubyInstaller](https://rubyinstaller.org/).

### 3. **Bundler** (gestor de dependencias de Ruby)  
Se instala con este comando en la terminal:

```bash
gem install bundler
```

---

## 🚀 Primeros pasos: ¡Clonar y ejecutar!

### Paso 1: Clonar este repositorio

Abre tu terminal (o Git Bash en Windows) y ejecuta:

\`\`\`bash
git clone https://github.com/tu-usuario/tu-repositorio.git
cd tu-repositorio
\`\`\`

> 🔁 Si estás empezando desde cero, puedes clonar directamente el tema Minimal Mistakes:

\`\`\`bash
git clone https://github.com/mmistakes/minimal-mistakes.git mi-sitio
cd mi-sitio
\`\`\`

### Paso 2: Instalar dependencias

Ejecuta este comando para instalar Jekyll y los plugins necesarios:

\`\`\`bash
bundle install
\`\`\`

> ⚠️ Si ves errores, prueba con \`bundle config set --local path 'vendor/bundle'\` antes de \`bundle install\`.

---

## ▶️ Iniciar el servidor local

Para ver tu sitio en tu navegador, ejecuta:

\`\`\`bash
bundle exec jekyll serve
\`\`\`

Luego abre tu navegador y visita:

👉 [http://localhost:4000](http://localhost:4000)

> ✅ ¡Verás tu sitio en vivo! Cada cambio que hagas en los archivos se recargará automáticamente (modo *watch*).

---

## 📁 Estructura básica del proyecto

Aquí te explico los archivos y carpetas más importantes:

\`\`\`
  mi-sitio/
  ├── _config.yml          ← Configuración principal del sitio (título, autor, redes, etc.)
  ├── _posts/              ← Aquí van tus entradas de blog (archivos .md)
  ├── _pages/              ← Páginas adicionales (sobre mí, contacto, etc.)
  ├── assets/              ← Imágenes, CSS, JS personalizados
  ├── Gemfile              ← Lista de dependencias (plugins, temas)
  └── index.html           ← Página de inicio
\`\`\`

---

## ✏️ Personalizar tu sitio

### 1. Editar \`_config.yml\`

Este es el **corazón de tu sitio**. Abrelo con cualquier editor de texto (VS Code, Sublime, Notepad++).

Ejemplo básico:

\`\`\`yaml
title: Mi Blog Personal
name: Tu Nombre
description: >- # esto permite saltos de línea
  Bienvenido a mi blog. Aquí escribo sobre tecnología, viajes y vida.
url: "http://localhost:4000" # cambia esto cuando subas a producción
baseurl: ""

# Autor
author:
  name: Tu Nombre
  bio: "Apasionado por el café y el código."
  avatar: "/assets/images/avatar.jpg" # coloca tu foto aquí
\`\`\`

> 💡 Cambia \`url\` por tu dominio real cuando lo publiques (ej: \`https://minombre.com\`).

---

### 2. Crear tu primera entrada de blog

Ve a la carpeta \`_posts/\` y crea un archivo con este formato:

\`\`\`
YYYY-MM-DD-titulo-de-mi-entrada.md
\`\`\`

Ejemplo: \`2025-04-05-mi-primer-post.md\`

Contenido del archivo:

\`\`\`markdown
---
title: "Mi primer post en Jekyll"
date: 2025-04-05
categories: [tecnología, tutoriales]
tags: [jekyll, ruby, principiantes]
---

¡Hola mundo! Este es mi primer post usando Jekyll y Minimal Mistakes.

Es muy fácil escribir en **Markdown**. Puedes usar:

- Negritas
- Cursivas
- Listas
- Enlaces
- Imágenes

¡Y mucho más!
\`\`\`

> 📌 Guarda el archivo y refresca tu navegador. ¡Tu post aparecerá automáticamente!

---

### 3. Crear páginas adicionales (ej: “Sobre mí”)

Crea un archivo en \`_pages/\`, por ejemplo: \`about.md\`

\`\`\`markdown
---
title: "Sobre mí"
permalink: /about/
---

¡Hola! Soy [Tu Nombre], y me encanta...

[...tu contenido aquí...]
\`\`\`

> 🔗 La página estará disponible en \`http://localhost:4000/about/\`

---

## 🎨 Personalizar el diseño

Minimal Mistakes es muy flexible. Puedes cambiar:

- Colores
- Fuentes
- Diseño de cabecera
- Sidebar
- Redes sociales

Todo se configura en \`_config.yml\` o en archivos dentro de \`_data/\`.

Ejemplo: agregar redes sociales

\`\`\`yaml
# _config.yml
author:
  links:
    - label: "Twitter"
      icon: "fab fa-twitter"
      url: "https://twitter.com/tuusuario"
    - label: "GitHub"
      icon: "fab fa-github"
      url: "https://github.com/tuusuario"
\`\`\`

> 🖼️ Los íconos usan [Font Awesome](https://fontawesome.com/icons). Puedes buscar el nombre del ícono que quieras.

---

## 🌐 Publicar tu sitio (gratis)

### Opción 1: GitHub Pages (recomendado para novatos)

1. Crea un repositorio en GitHub llamado \`tu-usuario.github.io\`
2. Sube tu proyecto:

\`\`\`bash
git remote set-url origin https://github.com/tu-usuario/tu-usuario.github.io.git
git add .
git commit -m "Mi primer sitio Jekyll"
git push -u origin main
\`\`\`

3. En \`_config.yml\`, asegúrate de tener:

\`\`\`yaml
url: "https://tu-usuario.github.io"
baseurl: ""
\`\`\`

4. Ve a **Settings > Pages** en tu repo de GitHub y selecciona la rama \`main\` (o \`gh-pages\` si usas esa).

👉 En unos minutos, tu sitio estará en: \`https://tu-usuario.github.io\`

---

### Opción 2: Netlify (más opciones, también gratis)

1. Sube tu código a cualquier repositorio en GitHub/GitLab.
2. Regístrate en [Netlify](https://www.netlify.com/).
3. Haz clic en “New site from Git”, selecciona tu repo.
4. En “Build command” pon: \`bundle exec jekyll build\`
5. En “Publish directory” pon: \`_site\`
6. ¡Listo! Netlify te dará una URL tipo \`tunombre.netlify.app\`

---

## ❓ Preguntas frecuentes (FAQ)

### ❓ ¿Necesito saber programar?

No. Solo necesitas saber editar archivos de texto y usar comandos básicos en la terminal. El contenido se escribe en **Markdown**, que es como escribir un mensaje de WhatsApp, pero con algunos símbolos para formato.

### ❓ ¿Qué es un archivo \`.md\`?

Es un archivo de texto con formato **Markdown**. Es super fácil:

\`\`\`markdown
# Título
## Subtítulo
**negrita**
*cursiva*
- lista
[enlace](https://ejemplo.com)
\`\`\`

### ❓ ¿Puedo usar imágenes?

¡Sí! Guárdalas en \`assets/images/\` y luego en tus posts:

\`\`\`markdown
![Texto alternativo](/assets/images/mi-imagen.jpg)
\`\`\`

### ❓ ¿Y si quiero cambiar el tema de colores?

Edita el archivo \`_sass/minimal-mistakes/_variables.scss\` o usa una skin predefinida en \`_config.yml\`:

\`\`\`yaml
minimal_mistakes_skin: "contrast" # o "default", "dark", "dirt", "mint", etc.
\`\`\`

---

## 🆘 ¿Algo no funciona?

- Revisa que **Ruby y Bundler** estén correctamente instalados.
- Ejecuta \`bundle update\` si hay errores de dependencias.
- Busca errores en la terminal cuando ejecutas \`bundle exec jekyll serve\`.
- Revisa la [documentación oficial de Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/).
- Únete a la comunidad en [GitHub Discussions](https://github.com/mmistakes/minimal-mistakes/discussions) o en foros como Reddit (\`r/jekyll\`).

---

## 📚 Recursos útiles

- [Documentación oficial de Jekyll (en español)](https://jekyllrb.com/docs/home/)
- [Guía rápida de Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/)
- [Cheatsheet de Markdown](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)
- [Editor de Markdown online](https://stackedit.io/)

---

## 💡 Consejos para novatos

1. **Haz backups**: Usa Git para guardar versiones (\`git add .\`, \`git commit -m "mensaje"\`, \`git push\`).
2. **Edita poco a poco**: Cambia una cosa a la vez y prueba en el navegador.
3. **Usa VS Code**: Es gratis y tiene extensiones para Jekyll y Markdown.
4. **No temas romper nada**: Siempre puedes volver atrás con Git o clonar de nuevo el tema.
5. **¡Diviértete!** Jekyll es una herramienta poderosa pero amigable.

---

## 🎉 ¡Listo! Ahora eres un creador de sitios con Jekyll

Con este proyecto puedes crear:

- Un blog personal
- Un portafolio profesional
- Una página de documentación
- Un diario digital
- ¡Lo que quieras!

> 🌟 **Recuerda: la mejor forma de aprender es haciendo.** Edita, prueba, rompe, arregla, vuelve a intentar.

---

## 📬 ¿Necesitas ayuda?

Abre un *issue* en este repositorio o contáctame (si aplica). ¡Estoy aquí para ayudarte!

---

⭐ **Si te gusta este proyecto, dale una estrella en GitHub.**  
☕ **¿Te sirvió? Invítame un café virtual.**

---

✅ Hecho con ❤️ y paciencia para principiantes.  
👨‍💻 Por [Tu Nombre o Usuario] — Abril 2025`;
