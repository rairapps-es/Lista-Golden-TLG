# Lista-Golden-TLG
Mini app en Telegram de Lista Golden.
# 🚀 MyAds Network - Telegram Mini App

¡Bienvenido al portal de contratación de publicidad automatizado! Esta es una **Telegram Mini App (TMA)** diseñada para funcionar de forma nativa dentro de Telegram, permitiendo a los anunciantes explorar mis canales, calcular presupuestos con combos/mejoras y generar pedidos en un solo clic.

---

## 🛠️ Características Principales

*   📱 **Diseño Pro Oscuro:** Optimizado para la interfaz móvil de Telegram.
*   🛒 **Cesta de la Compra Avanzada:** Permite añadir múltiples canales y aplicar mejoras (Packs, Mensajes Fijados).
*   ⭐ **Sistema de Favoritos:** Persistencia de datos local mediante `LocalStorage` (los datos no se borran al cerrar la app).
*   🔍 **Filtros Inteligentes:** Clasificación por categorías y ordenación por precios o volumen de suscriptores.
*   💬 **Checkout Directo:** Genera una plantilla de pedido estructurada y redirige al cliente a mi chat privado de Telegram.

---

## ⚙️ Cómo Personalizar los Canales (Para Mí)

Para añadir, quitar canales o cambiar los precios, solo debes editar el archivo `index.html` y buscar la constante `canalesData` (alrededor de la línea 130). 

Cada canal tiene la siguiente estructura que puedes modificar:

```javascript
{
    id: 1,                          // ID único numérico
    nombre: "Nombre del Canal",
    username: "usuario_sin_arroba",
    categoria: "Finanzas",          // Categoría para el filtro
    subs: 45000,                    // Número de suscriptores
    precioBase: 50,                 // Precio en USD
    descuento: 15,                  // % de descuento (0 si no tiene)
    oferta: true,                   // true para que aparezca en la pestaña "Ofertas"
    imagen: "URL_de_la_foto",
    descripcion: "Texto descriptivo...",
    duracion: "24 horas",
    fijado: "Sí, 2 horas"
}

© 2026 Lista Golden. Todos los derechos reservados.
