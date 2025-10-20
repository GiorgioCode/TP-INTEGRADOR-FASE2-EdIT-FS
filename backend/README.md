# 🎮 GameHub Backend - JSON Server API

Backend del proyecto GameHub E-commerce que utiliza JSON Server para simular una API REST completa con productos gaming y gestión de órdenes.

## 🚀 Inicio Rápido

### Instalación

```bash
npm install
```

### Ejecución

```bash
# Modo desarrollo (con auto-reload)
npm run dev
# o
npm start
```

El servidor se ejecutará en: **http://localhost:3001**

## 📡 Endpoints disponibles

### Productos
- **GET** `/products` - Obtener todos los productos
- **GET** `/products/:id` - Obtener un producto específico
- **POST** `/products` - Crear un nuevo producto
- **PUT** `/products/:id` - Actualizar un producto
- **DELETE** `/products/:id` - Eliminar un producto

### Órdenes de compra
- **GET** `/orders` - Obtener todas las órdenes
- **GET** `/orders/:id` - Obtener una orden específica  
- **POST** `/orders` - Crear una nueva orden de compra
- **PUT** `/orders/:id` - Actualizar una orden
- **DELETE** `/orders/:id` - Eliminar una orden

### Parámetros de consulta disponibles
- `_page` - Paginación
- `_limit` - Límite de resultados
- `_sort` - Ordenar por campo
- `_order` - Orden ascendente (asc) o descendente (desc)
- `q` - Búsqueda de texto completo

## 📊 Estructura de datos

### Producto
```json
{
  "id": 1,
  "nombre": "PlayStation 5 Slim",
  "descripcion": "Consola Sony PlayStation 5 Slim con SSD 1TB...",
  "precio": 899999,
  "imagen": "https://images.unsplash.com/..."
}
```

### Orden de compra
```json
{
  "id": 1,
  "productos": [
    {
      "id": 1,
      "nombre": "PlayStation 5 Slim",
      "precio": 899999,
      "cantidad": 2
    }
  ],
  "total": 1799998,
  "fecha": "2025-10-20T00:00:00.000Z"
}
```

## 🎮 Productos disponibles

La base de datos incluye 8 productos gaming:
- Consolas (PlayStation 5, Xbox Series X, Steam Deck)
- Periféricos (teclados, mouse, auriculares)
- Componentes (tarjetas gráficas)
- Monitores gaming

## 🔧 Configuración

- **Puerto**: 3001 (configurable en package.json)
- **Base de datos**: `db.json`
- **Watch mode**: Habilitado (cambios en db.json se reflejan automáticamente)

## 🛠️ Tecnologías

- **json-server**: ^0.17.4
- **Node.js**: Runtime de JavaScript

## 📝 Notas

- Los cambios en la base de datos se guardan automáticamente en `db.json`
- Para reiniciar la base de datos, eliminar las órdenes del archivo `db.json`
- CORS está habilitado por defecto en JSON Server
