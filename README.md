# OriginDev

**OriginDev** es un portfolio/landing page para un equipo de desarrolladores Full Stack, construido con **Next.js 15** y **Tailwind CSS 4**. Presenta a los miembros del equipo en un carrusel interactivo, permite explorar el perfil detallado de cada desarrollador, simula un carrito de "contratación" de perfiles, e incluye un formulario de registro de usuario — todo con soporte de tema claro/oscuro.

## ✨ Funcionalidades

- **Carrusel de desarrolladores** — navegación con flechas y teclado (`←` `→`), scroll suave y cards independientes.
- **Perfiles desplegables** — cada card permite ver el detalle del desarrollador (stack, nivel, disponibilidad, modalidad de trabajo) sin afectar el layout de las demás.
- **Carrito de contratación** — agregá desarrolladores a un carrito persistente (vía `localStorage`), con contador en el ícono de navbar.
- **Tema claro / oscuro** — toggle global persistente entre sesiones.
- **Formulario de usuario** — página de registro/login (`/FormUser`) con validación básica.
- **Buscador de país** — filtro en tiempo real para seleccionar país de origen.
- **Diseño responsive** — navbar adaptable con menú hamburguesa en pantallas chicas.

## 🛠️ Stack técnico

| Categoría | Tecnología |
|---|---|
| Framework | [Next.js 15](https://nextjs.org/) (Pages Router) |
| UI | [React 19](https://react.dev/) |
| Estilos | [Tailwind CSS 4](https://tailwindcss.com/) |
| Animaciones | [Framer Motion](https://www.framer.com/motion/) |
| Iconos | [React Icons](https://react-icons.github.io/react-icons/) |
| Persistencia | `localStorage` (tema y carrito) |
| Deploy | [Vercel](https://vercel.com/) |

## 📁 Estructura del proyecto

```
src/
├── components/       # Componentes UI (Navbar, Cards, Footer, formularios, etc.)
├── contexts/         # Contextos globales: ThemeContext y CarritoContext
├── hooks/            # Custom hooks
├── pages/            # Rutas de Next.js (Pages Router)
│   ├── api/          # API routes
│   ├── index.js      # Home
│   ├── carrito.jsx   # Vista del carrito
│   └── FormUser.js   # Formulario de usuario
├── styles/           # Estilos globales
└── utils/            # Componentes y funciones utilitarias
public/
└── img/              # Imágenes y assets estáticos
```

## 🚀 Cómo correrlo localmente

```bash
# Instalar dependencias
npm install

# Levantar el servidor de desarrollo
npm run dev
```

Abrí [http://localhost:3000](http://localhost:3000) para ver el resultado.

### Otros comandos

```bash
npm run build   # build de producción
npm run start   # levantar el build de producción
npm run lint    # correr el linter
```

## 📦 Deploy

El proyecto está configurado para desplegarse directamente en [Vercel](https://vercel.com/), que detecta Next.js automáticamente. Incluye un `vercel.json` con configuración explícita de framework, comandos de build y región de despliegue.

## 👥 Autores

Proyecto desarrollado en conjunto por estudiantes y profesores de la carrera Full Stack Developer de **Global Academy**.