# 🧁 The late Glaze

Sitio web de catálogo y pedidos para **The late Glaze**, una repostería artesanal de cupcakes, pasteles, roles de canela y más. El cliente arma su pedido desde el celular y lo envía por WhatsApp con el resumen ya escrito; la dueña administra productos, precios, disponibilidad y pedidos desde un panel protegido.

> **Estado:** 🚧 en desarrollo. 

## El problema

La repostería recibe hoy sus pedidos por WhatsApp e Instagram, lo que implica:

- Estar pendiente de los mensajes todo el tiempo.
- Enviar el catálogo y los datos de cuenta una y otra vez.
- Reunir por mensajes sueltos la información de cada pedido (productos, fecha, lugar de entrega, notas).

## La solución

Un sitio web optimizado para celular donde:

1. El cliente ve el catálogo con fotos y precios.
2. Arma su pedido y llena un formulario de entrega.
3. El pedido se guarda en la base de datos y se abre WhatsApp con el resumen listo para enviar.
4. La dueña gestiona todo desde un panel de administración, sin tocar código.

## Funcionalidades

- [ ] Catálogo de productos con foto, descripción, categorías y precio
- [ ] Carrito y formulario de pedido (con validación de 3 días de anticipación)
- [ ] Envío del pedido por WhatsApp (enlace `wa.me`) y guardado en MongoDB
- [ ] Panel de administración protegido por login
- [ ] Gestión de productos, precios y disponibilidad
- [ ] Gestión de pedidos y su estado
- [ ] Carrusel de testimonios en la página de inicio
- [ ] Diseño mobile-first y SEO básico

## Stack

| Capa | Tecnología |
|---|---|
| Frontend | HTML, CSS y JavaScript |
| Backend | Node.js + Express |
| Base de datos | MongoDB Atlas |
| Control de versiones | Git y GitHub |
| Despliegue | _por definir_ |

### Decisiones técnicas

- **HTML/CSS/JS plano, sin framework de frontend:** el objetivo del proyecto es aprender cómo se conectan navegador, API y base de datos, y un framework ocultaría parte de ese flujo.
- **Express sirve el sitio y la API:** un solo proyecto y un solo servidor son más fáciles de desplegar y mantener.
- **WhatsApp con enlace `wa.me` y no con la API oficial:** es gratuito y suficiente para la versión 1.
- **Precios calculados en el servidor:** el servidor nunca confía en los precios que envía el navegador.

## Estructura del proyecto

> Estructura prevista; se actualizará conforme avance el desarrollo.

```
the-late-glaze/
├── public/          # Sitio: HTML, CSS, JS e imágenes
├── server/          # API con Express
│   └── index.js
├── docs/            # Documentación y capturas
├── .env.example     # Variables de entorno de ejemplo (sin valores reales)
├── .gitignore
├── package.json
└── README.md
```

## Documentación

- Documento de requerimientos de software: _se agregará en `docs/`_


## Qué estoy aprendiendo con este proyecto

<!-- TODO: completar al terminar cada etapa: API REST, conexión a MongoDB, autenticación, validación, despliegue -->
_Se completará durante el desarrollo._

## Autor

**Angel Marco** — estudiante de desarrollo de software
GitHub: [@angelcobos380-art](https://github.com/angelcobos380-art)

Proyecto desarrollado para un cliente real y como parte de mi portafolio.
