# Checklist: Contenido

La siguiente es una lista de las condiciones que debe cumplir un sitio web para mantener el estándar de calidad de **Brand Industry.** Estas partes deben ser consideradas desde el inicio del proceso, **incluyendo estructura y maquetación**, y deben ser complementadas con los requerimientos específicos de cada cliente.

### Índice

- [Header](#1-Header)
- [Vistas](#2-Vistas)
	- [General](#21-General)
	- [Productos](#22-Productos)
- [Footer](#3-Footer)

## Header

- Logo (cambiar en móvil si es necesario)
- Datos de contacto
	- Link a Maps, usando *My location* como en [este ejemplo]("https://www.google.com/maps?saddr=My+Location&daddr=CONTYQUIM")
	- Link para llamada telefónica: `<a href="tel:..."></a>`
	- Link a correo: `<a href="mailto:..."></a>`
- Call to Action
- UX/UI
	- Mostrar/esconder el header al hacer scroll
	- Hamburguesa animada (móvil)

## Vistas

Las vistas que requiere un sitio web dependerán del tipo de sitio que se esté desarrollando:

### General

Todos los sitios **sin excepción** deben contepmplar las siguientes vistas:

- Home
	- Jumbotron
		- Call to Action
- Nosotros / Quiénes somos / Conócenos
- Servicios
- Landings de servicios, utilizar el [Cuestionario para Landing Page](#)
- *Partial* de contacto (no vista completa)
	- Datos de contacto
		- Link a Maps, usando la función *My location* como en [este ejemplo]("https://www.google.com/maps?saddr=My+Location&daddr=CONTYQUIM")
		- Link para llamada telefónica: `<a href="tel:..."></a>`
		- Link a correo: `<a href="mailto:..."></a>`
		- Links a redes sociales
	- Formulario de contacto
		- Nombre
		- Correo
		- Teléfono
		- Mensaje
		- El formulario debe ser validado mediante el attributo `required` en los campos **y por medio de Javascript.**
		- Respuesta en vivo (ajax/axios)
	- API Google Maps adecuado al *look and feel* del sitio web
		- Añadir un marker por cada sucursal del cliente. Cada marker debe contar con *info window* que tenga la información de la sucursal correspondiente
- Blog
	- *Partials*
		- Sidebar
			- Categorías
			- Mini grid (entradas destacadas)
		- Grid
			- Entrada
				- Imagen destacada
				- Título
				- Resumen
				- Categoría
			- Paginación
	- Main
		- Jumbotron/slider con entradas destacadas o más recientes
		- Ambos *Partials*
	- Categoría
		- *Breadcrumbs*
		- Ambos *Partials*
	- Single
		- *Breadcrumbs*
		- Información del artículo: autor, fecha, categoría...
		- Contenido
		- Artículos relacionados
		- [Disqus](https://disqus.com/)

### Productos

Los sitios web que contengan información específica sobre productos requerirán una estructura más amplia, por lo que las siguientes vistas son necesarias:

- *Partials*
	- Sidebar
		- Filtros por categoría y/o marca y/o industria
		- Buscador
	- Grid
		- Producto
			- Imagen destacada
			- Título
			- Categoría / marca
			- Precio, en caso de que aplique
		- Paginación

- Productos
	- Ambos *partials*
	- Slider (más productos/marcas/industrias/categorías)
- Categoría
	- *Breadcrumbs*
	- Ambos *partials*
	- Slider (más productos/marcas/industrias/categorías)
- Cotizador
	- Ambos *partials*, con las funciones adaptadas al cotizador (en lugar de llevar al *Single*, irá poblando una lista de productos a cotizar)
	- Formulario de contacto
		- Nombre
		- Correo
		- Teléfono
		- Mensaje
		- El formulario debe ser validado mediante el attributo `required` en los campos **y por medio de Javascript.**
		- Respuesta en vivo (ajax/axios)

*Además, buscará conseguirse información adicional tan temprano como se pueda en el proceso, con el objetivo de tener Landing Pages para temáticas como __Soporte__ o __Distribuidores__*

## Footer

- Logo
- Párrafo descriptivo de la empresa
- Links a redes sociales
- Navegaciones:
	- Del sitio
	- De servicios o categorías de productos
- Datos de contacto
	- Link a Maps, usando la función *My location* como en [este ejemplo]("https://www.google.com/maps?saddr=My+Location&daddr=CONTYQUIM")
	- Link para llamada telefónica: `<a href="tel:..."></a>`
	- Link a correo: `<a href="mailto:..."></a>`