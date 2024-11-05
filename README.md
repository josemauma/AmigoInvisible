# Amigo Invisible Automático 🎅🤫

Este proyecto en Python organiza un "Amigo Invisible" de forma automatizada, asignando aleatoriamente un amigo invisible a cada participante y notificándolos por correo electrónico. Ideal para grupos de amigos, familiares o equipos de trabajo que quieran gestionar su intercambio de regalos sin complicaciones.

## Características

- **Asignación Aleatoria**: Asigna un amigo invisible a cada participante asegurando que nadie se asigne a sí mismo.
- **Envío de Correos Automático**: Utiliza el protocolo SMTP para enviar correos personalizados con las asignaciones.
- **Gestión Segura de Credenciales**: Carga las credenciales del remitente desde un archivo `.env` para proteger la información.
- **Interfaz en Consola**: Imprime las asignaciones en la consola para una revisión rápida (opcional).

## Estructura del Código

1. **Importación de Librerías**: Usa librerías para el manejo de correos, aleatorización y lectura de archivos.
2. **Carga de Credenciales**: Carga el correo y la contraseña del remitente desde un archivo `.env`.
3. **Funciones Principales**:
   - `asignar_amigos`: Realiza la asignación aleatoria de amigos invisibles.
   - `enviar_correos`: Envía los correos electrónicos a cada participante con su amigo asignado.
   - `imprimir_asignaciones`: Muestra en consola las asignaciones para revisión.
4. **Función `main`**: Coordina el flujo general, desde cargar los datos hasta enviar los correos.

## Archivos Requeridos

- `Information.env`: Archivo de variables de entorno que contiene las credenciales de correo del remitente:
  ```plaintext
  EMAIL_REMITENTE=<tu_email>
  CONTRASENA_REMITENTE=<tu_contraseña>

## Requisitos

1. **Python 3**
   
2. **Paquetes de python:**
  - `random`
  - `smtplib`
  - `pandas`
  - `email`
  - `dotenv`

3. **Archivos de configuración:**
     `.env` con las credenciales del remitente y un archivo CSV (`Name_Email.csv`) con los nombres y correos de los participantes.

## Ejecución

Para ejecutar el script, asegúrate de tener los archivos necesarios (`Information.env` y `Name_Email.csv`) y luego ejecuta el siguiente comando en tu terminal:
```plaintext
python Amigo_Invisible.py

