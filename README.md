# 🎮 GameHub - E-commerce Gaming

Proyecto completo de e-commerce desarrollado con React + Vite (frontend) y JSON Server (backend), especializado en productos gaming (consolas, periféricos y componentes) con funcionalidades de carrito de compras y gestión de pedidos.

## 🛠️ Tecnologías Utilizadas

### Frontend

-   **React 19** - Biblioteca de JavaScript para interfaces de usuario
-   **Vite** - Herramienta de construcción rápida y moderna
-   **Zustand** - Gestión de estado global minimalista
-   **React Router DOM** - Enrutamiento del lado del cliente
-   **TailwindCSS** - Framework de utilidades CSS para diseño moderno

### Backend

-   **JSON Server** - API REST simulada para desarrollo rápido
-   **Node.js** - Entorno de ejecución para JavaScript

## 📁 Estructura del Proyecto

```
clase41/
├── backend/                    # Servidor JSON con API REST
│   ├── db.json                # Base de datos con productos y órdenes
│   ├── package.json           # Dependencias del backend
│   └── README.md              # Documentación del backend
├── frontend/                   # Aplicación React
│   ├── src/
│   │   ├── components/        # Componentes reutilizables
│   │   │   ├── Cart.jsx       # Carrito de compras
│   │   │   ├── Header.jsx     # Navegación principal
│   │   │   ├── ProductCard.jsx # Tarjeta de producto
│   │   │   └── ProductList.jsx # Lista de productos
│   │   ├── pages/             # Páginas principales
│   │   │   ├── Home.jsx       # Página de inicio
│   │   │   └── Products.jsx   # Catálogo de productos
│   │   ├── services/          # Servicios de API
│   │   │   └── api.js         # Comunicación con JSON Server
│   │   ├── store/             # Estado global
│   │   │   └── useCartStore.js # Store del carrito con Zustand
│   │   ├── App.jsx            # Componente principal
│   │   ├── App.css            # Estilos principales
│   │   └── main.jsx           # Punto de entrada
│   └── package.json           # Dependencias del frontend
└── README.md                  # Este archivo
```

## 🚀 Instalación y Ejecución

### 1. Instalar Dependencias

#### Backend

```bash
cd backend
npm install
```

#### Frontend

```bash
cd frontend
npm install
```

### 2. Ejecutar los Servidores

#### Backend (JSON Server) - Terminal 1

```bash
cd backend
npm run dev
```

El servidor estará disponible en: http://localhost:3001

#### Frontend (React + Vite) - Terminal 2

```bash
cd frontend
npm run dev
```

La aplicación estará disponible en: http://localhost:5173

## 📋 Funcionalidades Implementadas

1. **✅ Proyecto React con Vite** - Configuración moderna y optimizada
2. **✅ Sitio E-commerce** - Tienda completa de productos gaming
3. **✅ Datos desde JSON Server** - API REST con productos (id, nombre, descripción, precio, imagen)
4. **✅ JSON Server Independiente** - Backend separado en carpeta propia
5. **✅ Carrito de Compras** - Agregar/quitar productos con tarjetas
6. **✅ Cálculo de Total** - Precio total dinámico y visible
7. **✅ Finalizar Compra** - Envío de órdenes al JSON Server
8. **✅ Zustand + LocalStorage** - Estado global persistente
9. **✅ React Router DOM** - Navegación entre páginas
10. **✅ Diseño Responsive** - UX fluida con TailwindCSS
11. **✅ Reutilización de Componentes** - Arquitectura modular
12. **✅ Estructura Organizada** - Separación clara de responsabilidades
13. **✅ Mejores Prácticas** - Código limpio y mantenible
14. **✅ Código Comentado** - Documentación completa
15. **✅ Coherencia de Productos** - Tienda especializada en gaming

## 🎯 Endpoints de la API

### Productos

-   `GET /products` - Obtener todos los productos
-   `GET /products/:id` - Obtener producto por ID
-   `POST /products` - Crear nuevo producto
-   `PUT /products/:id` - Actualizar producto
-   `DELETE /products/:id` - Eliminar producto

### Órdenes

-   `GET /orders` - Obtener todas las órdenes
-   `GET /orders/:id` - Obtener orden por ID
-   `POST /orders` - Crear nueva orden (checkout)
-   `PUT /orders/:id` - Actualizar orden
-   `DELETE /orders/:id` - Eliminar orden

## 💾 Persistencia de Datos

### Carrito de Compras

-   **LocalStorage** - Los productos se mantienen entre sesiones
-   **Zustand Store** - Estado global reactivo
-   **Sincronización** - Estado consistente en toda la aplicación

### Base de Datos

-   **db.json** - Archivo JSON con productos y órdenes
-   **Auto-guardado** - JSON Server guarda automáticamente los cambios

## 🖥️ Navegación

-   **/** - Página de inicio con productos destacados
-   **/products** - Catálogo completo con filtros
-   **/about** - Información de la empresa
-   **Carrito** - Accesible desde cualquier página (overlay)

## 📱 Diseño Responsive

-   **Desktop** - Grid de 3-4 productos por fila
-   **Tablet** - Grid de 2-3 productos por fila
-   **Mobile** - Lista de 1 producto por fila
-   **Carrito** - Sidebar responsivo que se adapta al dispositivo

## 🔧 Configuración de Desarrollo

### Scripts Disponibles

#### Backend

-   `npm run dev` - Inicia JSON Server en modo desarrollo
-   `npm start` - Inicia JSON Server en modo producción

#### Frontend

-   `npm run dev` - Inicia servidor de desarrollo con Vite
-   `npm run build` - Construye la aplicación para producción
-   `npm run preview` - Previsualiza la build de producción

### URL DE Ejecución

La aplicación está configurada para funcionar con:

-   **Backend URL**: http://localhost:3001
-   **Frontend URL**: http://localhost:5173

## 🛡️ Manejo de Errores

-   **Servidor Desconectado** - Mensaje informativo con instrucciones
-   **Productos No Encontrados** - Estado vacío con opciones de retry
-   **Error de Checkout** - Feedback claro sobre fallos en el proceso
-   **Imágenes Rotas** - Placeholder automático para imágenes no válidas

## 🎨 Paleta de Colores (Gaming Theme)

-   **Primario**: #3B82F6 (Azul eléctrico)
-   **Secundario**: #10B981 (Verde gaming)
-   **Acento**: #EF4444 (Rojo acción)
-   **Fondo**: #F9FAFB (Gris claro)
-   **Texto**: #111827 (Negro profundo)

---
