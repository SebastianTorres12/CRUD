# Actividad Práctica CRUD

 La plataforma proporciona una experiencia de gestión integral para una tienda, facilitando las operaciones fundamentales de Crear, 
 Leer, Actualizar y Eliminar (CRUD). Con un enfoque simple y eficiente, los usuarios pueden administrar clientes, productos y pedidos, 
 cada uno con su respectivo detalle. La web se centra en la relación uno a varios, permitiendo a los usuarios añadir, editar y eliminar 
 información con facilidad.

## Paquetes y Herramientas Utilizadas

- ** Entity Framework Core:** `Microsoft.EntityFrameworkCore.SqlServer` se utiliza para realizar operaciones de base de datos de manera eficiente y simplificada
- ** Entity Framework Design:** `Microsoft.EntityFrameworkCore.Design` para crear migraciones y actualizar la base de datos.
- ** Entity Framework SQL Server:** `Microsoft.EntityFrameworkCore.SqlServer` para la conexión y operaciones con SQL Server.
- ** VisualStudio Web CodeGeneration:** `Microsoft.EntityFrameworkCore.SqlServer` se utiliza para generar código automáticamente en proyectos web de ASP.NET.

# Estructura del Proyecto

La estructura del proyecto sigue la arquitectura MVC (Modelo-Vista-Controlador), con algunos puntos clave:

- **Controllers:** Carpeta que contiene los controladores de la aplicación.
- **Data:** Carpeta que almacena las clases de entidades y el contexto de la base de datos.
- **Migrations:** Carpeta que incluye las migraciones de la base de datos para cambios controlados.
- **Models:** Carpeta que contiene las clases de modelo para las entidades del negocio.
- **Views:** Carpeta que aloja las vistas de la aplicación.

# Instrucciones para Ejecutar el Proyecto

## Configuración Inicial

1. **Clonar o descargar el Repositorio:**
   - Clona este repositorio en tu máquina local usando el siguiente comando:
     ```bash
     git clone <URL_del_repositorio>
     ```

2. **Abrir el Proyecto:**
   - Abre la solución del proyecto en Visual Studio (.sln).

3. **Configuración de la Base de Datos:**
   - Abre el archivo `appsettings.json` en el proyecto.
   - Modifica la cadena de conexión bajo la clave `"ConnectionStrings"` según tu entorno y configuración de SQL Server.

4. **Actualizar la Base de Datos:**
   - Abre la consola del administrador de paquetes NuGet y ejecuta el siguiente comando para aplicar migraciones y actualizar la base de datos:
     ```bash
     dotnet ef database update
     ```
   - Este comando asegura que la base de datos esté configurada con las últimas migraciones.

## Ejecutar la Aplicación

1. **Iniciar la Aplicación:**
   - Presiona F5 o elige "Start Debugging" en Visual Studio para iniciar la aplicación.

2. **Interactuar con el CRUD:**
   - Explora las secciones de Clientes, Productos y Pedidos para realizar operaciones CRUD.

## ¡Listo!
