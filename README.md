# {{NOMBRE_EMPRESA}} - Sitio Web Corporativo

Sitio web corporativo minimalista y elegante construido con Next.js, TypeScript, Tailwind CSS y Framer Motion.

## 🚀 Inicio Rápido

\`\`\`bash
# Instalar dependencias
npm install

# Ejecutar en desarrollo
npm run dev

# Construir para producción
npm run build

# Ejecutar en producción
npm start
\`\`\`

Abre [http://localhost:3000](http://localhost:3000) en tu navegador.

## 🎨 Personalización

### 1. Información de la Empresa

Edita `config/site.ts` y reemplaza los placeholders:

\`\`\`typescript
export const siteConfig = {
  name: "Tu Empresa", // Reemplazar {{NOMBRE_EMPRESA}}
  alias: "TuEmpresa", // Reemplazar {{ALIAS}}
  // ... resto de configuración
}
\`\`\`

### 2. Colores y Tema

Edita `styles/globals.css` y reemplaza los colores:

\`\`\`css
/* Reemplazar {{HEX_PRINCIPAL}} y {{HEX_ACENTO}} */
--color-brand: #1a56db; /* Tu color principal */
--color-accent: #0ea5e9; /* Tu color de acento */
\`\`\`

### 3. Contenido

Los datos del sitio están en la carpeta `/data`:

- `services.ts` - Servicios ofrecidos
- `projects.ts` - Casos de éxito
- `testimonials.ts` - Testimonios de clientes
- `tech.ts` - Stack tecnológico

### 4. Imágenes y Logos

Reemplaza los placeholders en `/public`:

- `/public/images/hero.jpg` - Imagen del hero
- `/public/images/cases/*.jpg` - Imágenes de casos de estudio
- `/public/logos/*.svg` - Logos de tecnologías

## 📧 Configurar Email

El formulario de contacto necesita un servicio de email. Recomendamos [Resend](https://resend.com).

1. Crea una cuenta en Resend
2. Obtén tu API key
3. Añade a `.env.local`:
   \`\`\`
   RESEND_API_KEY=tu_api_key
   \`\`\`
4. Descomenta el código en `lib/email.ts`
5. Instala Resend: `npm install resend`

## 📁 Estructura del Proyecto

\`\`\`
/app                    # Páginas y rutas
  /page.tsx            # Página principal
  /servicios           # Página de servicios
  /proyectos           # Página de proyectos
  /nosotros            # Página sobre nosotros
  /contacto            # Página de contacto
  /api                 # API routes
/components            # Componentes React
  /ui                  # Componentes UI base
  /layout              # Navbar, Footer
  /cards               # Cards de features, casos, testimonios
  /hero                # Hero section
  /logos               # Marquee de tecnologías
  /forms               # Formularios
/data                  # Datos del sitio
/lib                   # Utilidades y helpers
/config                # Configuración del sitio
/styles                # Estilos globales
/public                # Assets estáticos
\`\`\`

## 🛠️ Stack Tecnológico

- **Framework**: Next.js 15 (App Router)
- **Lenguaje**: TypeScript
- **Estilos**: Tailwind CSS v4
- **Componentes**: shadcn/ui
- **Animaciones**: Framer Motion
- **Validación**: Zod
- **Formularios**: React Hook Form

## 📱 Características

- ✅ Diseño responsive (mobile-first)
- ✅ Modo claro/oscuro
- ✅ SEO optimizado
- ✅ Accesibilidad (WCAG AA)
- ✅ Animaciones sutiles
- ✅ Rendimiento optimizado
- ✅ TypeScript estricto

## 🎯 SEO

El sitio incluye:

- Metadata optimizada por página
- Open Graph images
- Sitemap.xml automático
- Robots.txt
- Structured data (JSON-LD)

## 📝 Añadir Casos de Estudio

1. Añade el proyecto a `data/projects.ts`
2. Crea un archivo MDX en `/content/proyectos/` (opcional)
3. Añade imágenes a `/public/images/cases/`

## 🚀 Despliegue

### Vercel (Recomendado)

1. Push tu código a GitHub
2. Importa el proyecto en [Vercel](https://vercel.com)
3. Configura las variables de entorno
4. ¡Despliega!

### Otros Proveedores

\`\`\`bash
npm run build
npm start
\`\`\`

## 📄 Licencia

Todos los derechos reservados © {{NOMBRE_EMPRESA}}

## 🤝 Soporte

Para soporte, contacta a: contacto@tuempresa.com

---

**TODO**: Antes de lanzar a producción:

- [ ] Reemplazar {{NOMBRE_EMPRESA}}, {{ALIAS}} en config/site.ts
- [ ] Cambiar colores {{HEX_PRINCIPAL}}, {{HEX_ACENTO}} en globals.css
- [ ] Añadir imágenes reales en /public
- [ ] Configurar servicio de email (Resend)
- [ ] Actualizar URLs y enlaces sociales
- [ ] Añadir Google Analytics (opcional)
- [ ] Configurar dominio personalizado
- [ ] Revisar y actualizar contenido en /data
