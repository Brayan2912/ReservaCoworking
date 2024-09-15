# Sistema de Gestión de Reservas de Espacios de Coworking

Este proyecto es una aplicación web backend desarrollada con Java Servlets para gestionar las reservas de espacios en un coworking. La aplicación permite a los usuarios reservar diferentes tipos de espacios, ver la lista de reservas y eliminar reservas existentes.

** Requisitos

- Java Development Kit (JDK) 8 o superior
- Apache Tomcat 9 o superior
- NetBeans IDE (opcional, pero recomendado)

** Instalación

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/Brayan2912/ReservaCoworking.git
**Importar el proyecto en NetBeans:
Abre NetBeans.
Selecciona File > Open Project.
Navega hasta la carpeta donde clonaste el repositorio y selecciona el proyecto.
**Configurar Apache Tomcat:
Asegúrate de tener Apache Tomcat instalado y configurado en NetBeans.
Ve a Tools > Servers y añade tu servidor Tomcat si aún no lo has hecho.
Desplegar la aplicación:
Haz clic derecho en el proyecto en NetBeans y selecciona Run.
**Uso
Página de Inicio
Accede a la página principal (index.html) para realizar una reserva o por el link http://localhost:8080/ReservaCoworking/index.html)
Completa el formulario con tu nombre, fecha de reserva, tipo de espacio y duración.
Procesar Reservas
El formulario será procesado por el ReservaServlet, que validará los datos y almacenará la reserva en una lista en memoria.
Recibirás una confirmación de la reserva con los detalles ingresados.
Lista de Reservas
Accede a ListaReservasServlet para ver todas las reservas almacenadas.
Cada reserva mostrará el nombre del usuario, fecha, espacio reservado y duración.
Eliminar Reservas
Desde la lista de reservas, puedes eliminar una reserva haciendo clic en el botón “Eliminar” junto a la reserva correspondiente.
La eliminación será procesada por el EliminarReservaServlet.
**Estructura del Proyecto
index.html: Página principal con el formulario de reserva.
ReservaServlet.java: Servlet para procesar y almacenar reservas.
ListaReservasServlet.java: Servlet para mostrar la lista de reservas.
EliminarReservaServlet.java: Servlet para eliminar reservas.
Reserva.java: Clase que representa una reserva.
