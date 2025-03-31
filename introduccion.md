# Introducción

## ¿Qué es la Programación Orientada a Objetos (POO)?
La **Programación Orientada a Objetos (POO)** es un paradigma de programación basado en la organización del código en **objetos**, que representan entidades del mundo real.  
Es importante porque permite crear software modular, reutilizable y fácil de mantener.

## Cuatro fundamentos de POO

### 1. Abstracción
Es la capacidad de representar elementos del mundo real en el código.  
Ejemplo: Un **"Auto"** puede representarse con atributos (marca, modelo) y métodos (arrancar, frenar).

### 2. Encapsulamiento
Protege los datos de un objeto, permitiendo acceso solo a través de métodos específicos.  
Ejemplo: Un **"Cajero Automático"** no permite acceso directo al dinero, solo mediante transacciones.

### 3. Herencia
Permite que una clase reutilice características de otra.  
Ejemplo: Un **"Auto Deportivo"** hereda de la clase **"Auto"**, pero añade características como mayor velocidad.

### 4. Polimorfismo
Permite que una misma acción tenga diferentes comportamientos según el objeto.  
Ejemplo: Un **"Animal"** puede hacer un sonido, pero cada tipo de animal emite un sonido diferente (perro: ladrido, gato: maullido).

## Requisitos iniciales del sistema

1. **Registro de usuarios:** El sistema debe permitir la creación y gestión de usuarios.  
2. **Gestión de turnos:** Los usuarios deben poder solicitar, cancelar y reprogramar turnos.  
3. **Notificaciones:** El sistema debe enviar recordatorios de turnos vía correo o mensaje.  
4. **Historial de turnos:** Se debe permitir consultar turnos pasados.  
5. **Control de acceso:** Solo usuarios registrados pueden acceder a ciertas funciones.


   Casos de uso
Caso 1
Registro de usuario
Actores involucrados: Usuario y sistema
Descripción breve: Permite a un nuevo usuario crear una cuenta en la plataforma.
Flujo principal de eventos
El usuario accede a la página de registro.
El usuario ingresa su información personal (nombre, correo, contraseña).
El sistema valida la información ingresada.
El sistema crea una nueva cuenta y envía un correo de confirmación.
El usuario recibe el correo y confirma su registro.
Precondiciones: El usuario no debe tener una cuenta existente.
Postcondiciones: El usuario tiene una cuenta activa en el sistema.
Caso 2
Inicio de Sesión
Actores involucrados: Usuario, Sistema
Descripción breve: Permite a un usuario registrado acceder a su cuenta.
Flujo principal de eventos:
El usuario accede a la página de inicio de sesión.
El usuario ingresa su correo y contraseña.
El sistema valida las credenciales.
El sistema redirige al usuario a su panel de control.
Precondiciones: El usuario debe tener una cuenta registrada.
Postcondiciones: El usuario está autenticado y tiene acceso a su cuenta.
Caso 3
Recuperación de Contraseña
Actores involucrados: Usuario, Sistema.
Descripción breve: Permite a un usuario recuperar su contraseña en caso de olvido.
Flujo principal de eventos:
El usuario accede a la opción de "Olvidé mi contraseña".
El usuario ingresa su correo electrónico.
El sistema envía un enlace de recuperación al correo proporcionado.
El usuario sigue el enlace y establece una nueva contraseña.
Precondiciones: El usuario debe haber registrado su correo en la cuenta.
Postcondiciones: El usuario ha restablecido su contraseña y puede iniciar sesión.
Caso 4
Realizar una Compra
Nombre del caso de uso: Realizar una Compra
Actores involucrados: Usuario, Sistema, Proveedor.
Descripción breve: Permite a un usuario realizar una compra de productos o servicios.
Flujo principal de eventos:
El usuario navega por el catálogo de productos.
El usuario selecciona un producto y lo añade al carrito.
El usuario procede al pago.
El sistema procesa el pago y confirma la compra.
El sistema envía un recibo al usuario.
Precondiciones: El usuario debe estar autenticado y tener un método de pago válido.
Postcondiciones: La compra se ha completado y el usuario recibe la confirmación.
Caso 5
Cierre de Sesión
Actores involucrados: Usuario, Sistema.
Descripción breve: Permite a un usuario cerrar su sesión en la plataforma.
Flujo principal de eventos:
El usuario selecciona la opción de cerrar sesión.
El sistema finaliza la sesión del usuario.
El sistema redirige al usuario a la página de inicio.
Precondiciones: El usuario debe estar autenticado.
Postcondiciones: El usuario ha cerrado sesión y no tiene acceso a su cuenta hasta que inicie sesión nuevamente
Boceto inicial del diseño de clases (#Boceto)
