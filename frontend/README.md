# 🎮 GameHub Frontend

Frontend de la aplicación GameHub E-commerce desarrollado con React + Vite, especializado en productos gaming con carrito de compras persistente y diseño moderno.

## 🛠️ Stack Tecnológico

- **React 19** - Biblioteca principal para UI
- **Vite** - Build tool ultrarrápido y dev server con HMR
- **Zustand** - Gestión de estado global minimalista
- **React Router DOM** - Enrutamiento SPA
- **TailwindCSS** - Framework de utilidades CSS para diseño moderno
- **Autoprefixer & PostCSS** - Procesamiento de CSS

## 📦 Dependencias Principales

```json
{
  "react": "^19.1.1",
  "react-dom": "^19.1.1",
  "zustand": "^4.4.1",
  "react-router-dom": "^6.17.0"
}
```

## 🚀 Scripts Disponibles

- `npm run dev` - Servidor de desarrollo en http://localhost:5173
- `npm run build` - Compilación optimizada para producción
- `npm run preview` - Vista previa del build de producción
- `npm run lint` - Análisis de código con ESLint

## 📁 Estructura del Proyecto

```
src/
├── components/       # Componentes reutilizables
│   ├── Cart.jsx     # Drawer del carrito
│   ├── Header.jsx   # Navegación principal
│   ├── ProductCard.jsx # Tarjeta de producto
│   └── ProductList.jsx # Grilla de productos
├── pages/           # Vistas/Páginas
│   ├── Home.jsx     # Landing page
│   ├── Products.jsx # Catálogo completo
│   └── About.jsx    # Información
├── services/        # Comunicación con API
│   └── api.js       # Cliente HTTP
├── store/           # Estado global
│   └── useCartStore.js # Store Zustand
├── App.jsx          # Componente raíz
├── main.jsx         # Punto de entrada
└── index.css        # Estilos globales y Tailwind
```

## 🎨 Características Principales

- **🛒 Carrito Persistente** - LocalStorage + Zustand
- **📱 Diseño Responsive** - Mobile-first con TailwindCSS
- **🎯 SPA Navigation** - React Router con lazy loading
- **🔄 Estado Global** - Zustand con middleware de persistencia
- **⚡ Hot Module Replacement** - Desarrollo ágil con Vite
- **🎨 Componentes Modulares** - Arquitectura reutilizable

## ⚙️ Requisitos del Sistema

1. **Backend API**: JSON Server corriendo en `http://localhost:3001`
2. **Node.js**: Versión 18 o superior
3. **Navegador**: Chrome 90+, Firefox 88+, Safari 14+, Edge 90+
4. **JavaScript**: Habilitado (requerido para React)

## 🚀 Instalación y Ejecución

```bash
# Instalar dependencias
npm install

# Iniciar servidor de desarrollo
npm run dev

# Abrir en el navegador
http://localhost:5173
```

## 🔗 Integración con Backend

El frontend se conecta automáticamente al backend en `http://localhost:3001`. Asegúrate de:

1. Tener el backend ejecutándose antes de iniciar el frontend
2. Verificar que el puerto 3001 esté disponible
3. La API base URL está configurada en `src/services/api.js`

## 🐛 Solución de Problemas

- **Error de CORS**: Verifica que el backend esté corriendo
- **Página en blanco**: Revisa la consola del navegador
- **Carrito vacío tras refresh**: Verifica localStorage en DevTools
