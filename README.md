# DishDash - App Restaurante

Aplicación de escritorio para la gestión de comandas en un restaurante/cafetería, desarrollada como **Trabajo de Fin de Grado del ciclo de Desarrollo de Aplicaciones Multiplataforma (DAM)**.

El proyecto está orientado a facilitar el trabajo diario de un establecimiento mediante la toma de comandas, gestión de mesas, productos, empleados y consulta del histórico de pedidos.


---

## Demostración

La aplicación dependía de una API REST y una base de datos alojadas en una máquina virtual, por lo que actualmente el proyecto se conserva principalmente como muestra de código, estructura y documentación del TFG.

Para ver el funcionamiento completo de la aplicación, se puede consultar la siguiente lista de reproducción:

[Ver demostración en YouTube](https://www.youtube.com/playlist?list=PLReKtYAVOuBcX2NNTSs7deYTFgj6xRjn-)

---

## Descripción del proyecto

**DishDash** es una aplicación de escritorio diseñada para gestionar el flujo de trabajo básico de un restaurante o cafetería.

La aplicación permite registrar pedidos de clientes, asignarlos a mesas, seleccionar camareros, cobrar comandas, administrar productos del menú, gestionar empleados y consultar un histórico de comandas ya finalizadas.

El objetivo principal del proyecto fue crear una herramienta visual, sencilla y práctica que ayudara a organizar el servicio del establecimiento y redujera errores en la toma y gestión de pedidos.

---

## Funcionalidades principales

### Comandas

- Toma de comandas desde una vista principal.
- Añadir productos a una comanda.
- Modificar cantidades de los productos seleccionados.
- Eliminar líneas concretas de una comanda.
- Borrar una comanda completa antes de registrarla.
- Cobrar una comanda directamente.
- Pasar una comanda a una mesa para cobrarla más adelante.
- Asignar camarero, mesa y número de personas.
- Validaciones para evitar registrar comandas incompletas.

### Gestión de comandas

- Visualización de comandas pendientes de cobro.
- Edición de comandas ya asignadas a mesa.
- Eliminación de comandas pendientes.
- Consulta detallada de los productos incluidos en una comanda.
- Cobro de comandas pendientes.

### Gestión de mesas

- Visualización y administración de mesas del establecimiento.
- Control de mesas ocupadas.
- Control de capacidad de mesas según el número de personas.
- Creación, edición y eliminación de mesas.
- Guardado de cambios en la base de datos.

### Gestión de productos

- Listado de productos disponibles.
- Filtrado de productos por categoría.
- Creación de nuevos productos.
- Edición de productos existentes.
- Eliminación de productos.
- Gestión de información como nombre, precio, unidades, categoría e imagen.

### Gestión de empleados

- Acceso protegido mediante validación de administrador.
- Listado de empleados.
- Visualización detallada de información del empleado.
- Creación de empleados.
- Edición de datos de empleados.
- Eliminación de empleados.
- Validaciones en campos como DNI y fecha.
- Gestión de imagen del empleado.

### Histórico

- Consulta de comandas ya cobradas.
- Visualización de detalles de comandas finalizadas.
- Eliminación de registros del histórico en caso de error.

### Manual de usuario

- Manual integrado en la aplicación.
- Documentación paso a paso con capturas sobre el uso de cada módulo.

---

## Tecnologías utilizadas

### Aplicación de escritorio

- **C#**
- **WPF**
- **.NET Framework**
- **MVVM**
- **XAML**

### Backend y datos

- **API REST desarrollada en Java**
- **Base de datos MySQL**

> La API y la base de datos formaban parte de la infraestructura original del proyecto, alojada en una máquina virtual. Actualmente no están incluidas como entorno funcional dentro de este repositorio.

---

## Arquitectura y organización

El proyecto está organizado siguiendo una estructura basada en separación de responsabilidades, utilizando el patrón **MVVM** para dividir la lógica de presentación, las vistas y los datos.

Estructura principal del proyecto:

```text
Proyecto-Restaurante/
├── Assets/             # Recursos visuales de la aplicación
├── Components/         # Componentes reutilizables de interfaz
├── Convertidores/      # Conversores utilizados en bindings de WPF
├── Mensajes/           # Mensajes internos entre vistas/modelos
├── Modelos/            # Clases de dominio de la aplicación
├── Servicios/          # Servicios de navegación, diálogo, API, etc.
├── Vistas/             # Vistas de la aplicación
└── VistasModelo/       # ViewModels asociados a las vistas
```

Esta estructura permite mantener separada la interfaz gráfica de la lógica de negocio y facilita la organización de las distintas partes de la aplicación.

---

## Estado actual del proyecto

Este proyecto fue desarrollado como TFG de DAM y actualmente se conserva como proyecto de portfolio.

La aplicación **no está preparada para ejecutarse directamente tras clonar el repositorio**, ya que dependía de una infraestructura externa compuesta por:

- API REST en Java.
- Base de datos MySQL.
- Máquina virtual alojada en la nube.

Por este motivo, el repositorio está orientado principalmente a mostrar:

- La estructura del proyecto.
- La organización del código.
- El uso de WPF y MVVM.
- La funcionalidad completa mediante vídeos de demostración.
- La documentación generada durante el desarrollo del TFG.

---

## Requisitos originales

Durante el desarrollo, la aplicación estaba pensada para ejecutarse en un entorno Windows con los siguientes requisitos mínimos:

- Windows 10 o superior.
- 4 GB de RAM o superior.
- 100 MB de espacio disponible.
- Resolución mínima de 1280x800 píxeles.
- Conexión a Internet estable.
- Procesador Intel Core i3 o equivalente.

---

## Objetivos del proyecto

Los principales objetivos del proyecto fueron:

- Desarrollar una aplicación de escritorio funcional con WPF.
- Aplicar el patrón MVVM en un proyecto real.
- Consumir una API REST desde una aplicación de escritorio.
- Gestionar información persistente mediante una base de datos MySQL.
- Crear una interfaz clara para la toma y gestión de comandas.
- Implementar validaciones y flujos de trabajo similares a los de un entorno real.
- Documentar el uso de la aplicación mediante un manual de usuario.

---

## Aprendizajes

Este proyecto me permitió reforzar conocimientos importantes de desarrollo de aplicaciones, especialmente en:

- Desarrollo de interfaces de escritorio con WPF y XAML.
- Organización de proyectos utilizando MVVM.
- Comunicación entre aplicación cliente y API REST.
- Gestión de datos relacionados con productos, empleados, mesas y comandas.
- Validación de formularios y control de estados de la interfaz.
- Creación de documentación funcional para usuarios finales.
- Desarrollo de un proyecto completo con una estructura cercana a una aplicación real.

---

## Autor

**Ian Tauzy**

Proyecto desarrollado como Trabajo de Fin de Grado del ciclo de **Desarrollo de Aplicaciones Multiplataforma (DAM)**.

