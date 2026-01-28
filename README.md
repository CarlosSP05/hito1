EcoCity - Proyecto Integrador (Hito 1)
Descripción del Proyecto

EcoCity es una aplicación móvil diseñada para permitir a los ciudadanos reportar incidencias urbanas (como baches, farolas rotas o acumulación de basura) en tiempo real. Los usuarios pueden registrar incidencias mediante un formulario, adjuntar fotos o notas de voz y compartir la ubicación precisa a través del GPS. Además, la aplicación incluye una función de autenticación para gestionar el acceso de los usuarios.

Este repositorio corresponde al Hito 1, donde se implementaron las funcionalidades básicas de la interfaz, la gestión de incidencias y el almacenamiento local en SQLite.

Objetivos del Hito 1

El objetivo principal del Hito 1 fue desarrollar la pantalla principal de la aplicación y garantizar que el sistema de gestión de incidencias funcione de manera eficiente, tanto en línea como fuera de línea. Las características implementadas son:

Pantalla de Login: El usuario debe autenticarse para acceder a la aplicación.

Gestión de Incidencias: Los usuarios pueden reportar incidencias, que se almacenan localmente en una base de datos SQLite.

Visualización de Incidencias: Las incidencias reportadas se muestran en una lista (RecyclerView).

Tecnologías Utilizadas

Lenguaje: Java

Base de Datos: SQLite (para almacenamiento local de incidencias)

UI: RecyclerView para mostrar las incidencias

Autenticación: SharedPreferences para gestionar el inicio de sesión

Pasos Realizados en el Hito 1
1. Diseño de la Interfaz

LoginActivity: Implementación de la pantalla de inicio de sesión para la autenticación de los usuarios.

MainActivity: Pantalla principal donde se visualizan todas las incidencias reportadas en un RecyclerView.

2. Gestión de la Base de Datos

Se configuró una base de datos SQLite para almacenar las incidencias de manera local en el dispositivo.

Se creó el DAO (Data Access Object) para gestionar las operaciones CRUD sobre la base de datos.

3. Autenticación de Usuario

La autenticación se gestiona mediante SharedPreferences, donde se almacena el estado del inicio de sesión. Si el usuario está autenticado, accede a la pantalla principal; si no, es redirigido a la pantalla de login.

Estructura del Proyecto

MainActivity.java: Actividad principal que gestiona la visualización de incidencias.

LoginActivity.java: Actividad que permite al usuario iniciar sesión.

Incidencia.java: Modelo de datos que representa una incidencia.

IncidenciaDAO.java: Clase que maneja la base de datos SQLite.

IncidenciaAdapter.java: Adaptador para mostrar las incidencias en el RecyclerView.

activity_main.xml: Layout para la pantalla principal.

activity_login.xml: Layout para la pantalla de inicio de sesión.

item_incidencia.xml: Layout para cada elemento de la lista de incidencias.
