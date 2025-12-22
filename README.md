# Portfolio Minimalista

Este proyecto es un portafolio web profesional y accesible, desarrollado con Astro y TypeScript, que permite mostrar tu experiencia, formación, habilidades y proyectos de manera clara y elegante. Incluye una lógica pensada para la accesibilidad, navegación rápida mediante atajos de teclado y una modalidad especial para imprimir tu currículum en PDF.

## ✨ Características principales

- **Accesibilidad**: Navegación optimizada para teclado y lectores de pantalla.
- **Modal de impresión**: Permite mostrar el CV en un formato limpio y listo para imprimir o guardar como PDF.
- **Personalización sencilla**: Solo edita el archivo `cv.json` para actualizar tu información.
- **Diseño minimalista y responsive**: Se adapta a cualquier dispositivo.
- **Atajos de teclado**: Gracias a la integración de Ninja Keys, puedes navegar y acceder a secciones rápidamente.
- **Stack moderno**: Astro, TypeScript y componentes reutilizables.

## 📁 Estructura del proyecto

```
/
├── public/
│   ├── favicon.svg
│   └── me.webp
├── src/
│   ├── components/
│   │   ├── KeyboardManager.astro
│   │   └── sections/
│   │       ├── About.astro
│   │       ├── Education.astro
│   │       ├── Experience.astro
│   │       ├── Hero.astro
│   │       ├── Languages.astro
│   │       ├── Projects.astro
│   │       ├── Skills.astro
│   │       └── Certification.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   ├── cv.d.ts
│   ├── env.d.ts
│   └── types.d.ts
├── cv.json
├── astro.config.mjs
├── package.json
└── README.md
```


## 🚀 Instalación, build y despliegue

1. **Clona el repositorio:**

```bash
git clone https://github.com/R-Mutt22/portfolio-minimalist.git
cd portfolio-minimalist
```


2. **Instala las dependencias:**

```bash
pnpm install
```

3. **Personaliza tu CV:**

Edita el archivo `cv.json` con tu información personal, experiencia, educación, certificaciones, habilidades y proyectos.


4. **Inicia el servidor de desarrollo:**

```bash
pnpm run dev
```

5. **Build para producción:**

```bash
pnpm astro build
```

6. **Previsualiza localmente con Cloudflare Pages:**

```bash
pnpm exec wrangler pages dev ./dist
```

7. **Despliegue en Cloudflare Pages:**

- Sube tu código a GitHub.
- Conecta el repo en Cloudflare Pages y usa:
	- **Build command:** `pnpm astro build`
	- **Output folder:** `dist`
	- **Install command:** `pnpm install`

Consulta la documentación oficial de Cloudflare Pages para detalles avanzados.

5. **Accede a tu portfolio:**

Abre [http://localhost:4321](http://localhost:4321) en tu navegador.

## 🖨️ Modalidad de impresión

Haz clic en el botón de impresión o usa el atajo de teclado correspondiente para abrir la modal de impresión. El diseño se adapta automáticamente para que puedas imprimir tu CV o guardarlo como PDF, sin elementos innecesarios.


## 🧑‍💻 Comandos útiles

| Comando                          | Acción                                              |
|----------------------------------|----------------------------------------------------|
| `pnpm run dev`                   | Inicia el servidor de desarrollo                    |
| `pnpm astro build`               | Genera la versión de producción en `./dist/`        |
| `pnpm exec wrangler pages dev`   | Previsualiza la versión Cloudflare Pages localmente |


## 🛡️ Accesibilidad, seguridad y buenas prácticas

- Navegación por teclado y soporte para lectores de pantalla.
- Modal de impresión accesible y fácil de usar.
- Código limpio y modular, fácil de mantener y ampliar.
- Content Security Policy (CSP) para mitigar XSS.
- Optimización de imágenes con sharp en build.
- Dependencias auditadas y sin vulnerabilidades conocidas.

## 📄 Licencia

MIT. Puedes usar, modificar y compartir este proyecto libremente.

---

¿Listo para destacar tu perfil profesional? ¡Personaliza, imprime y comparte tu portfolio minimalista!


