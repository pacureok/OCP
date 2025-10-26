# OCP comand:
🛠️ Códigos de Uso Común en Herramientas de Compilación (OCP.exe hipotético)
Cuando una herramienta como OCP.exe orquesta la compilación, suele aceptar comandos para controlar las diferentes fases del proceso: limpiar, construir y ejecutar.

1. Construir/Compilar el Proyecto
Comando: OCP.exe build

Español: Construir o Compilar

Inglés: Build or Compile

Propósito: Este es el comando principal. Le indica a la herramienta que ejecute todos los pasos necesarios para crear el producto final (tu archivo .iso). Típicamente, esto incluye llamar a nasm.exe (ensamblar), ld.exe (enlazar), y xorriso.exe (crear el ISO).

Ejemplo: OCP.exe build

2. Limpiar el Proyecto
Comando: OCP.exe clean

Español: Limpiar

Inglés: Clean

Propósito: Elimina todos los archivos temporales y generados (como archivos .o, .bin, y el .iso final) para asegurar que la próxima construcción sea completamente nueva y no use archivos obsoletos.

Ejemplo: OCP.exe clean

3. Reconstruir/Forzar una Nueva Compilación
Comando: OCP.exe rebuild

Español: Reconstruir

Inglés: Rebuild

Propósito: Es una combinación de los dos comandos anteriores. Primero llama a clean para eliminar todo, y luego llama a build para construir el proyecto desde cero. Esto garantiza una compilación limpia.

Ejemplo: OCP.exe rebuild

4. Ejecutar el Sistema Operativo
Comando: OCP.exe run

Español: Ejecutar

Inglés: Run

Propósito: Este comando se utiliza después de una compilación exitosa. Inicia el emulador (como QEMU o VirtualBox) y carga tu archivo .iso para que puedas probar el sistema operativo.

Ejemplo: OCP.exe run

5. Ayuda o Documentación
Comando: OCP.exe help o OCP.exe -h o OCP.exe /?

Español: Ayuda

Inglés: Help

Propósito: Muestra el listado completo de comandos disponibles, sus parámetros opcionales, y cómo usar la herramienta. Este es el comando que necesitas usar primero, una vez que estés en la carpeta correcta.

Ejemplo (lo que necesitas ejecutar):

cd C:\Users\DELL\Downloads\ocp (O la ruta correcta)

OCP.exe help

Recordatorio: Primero, asegúrate de que el Símbolo del Sistema esté abierto en la carpeta exacta donde copiaste OCP.exe.

Bash

cd C:\Users\DELL\Downloads\ocp
Luego, prueba los comandos de ayuda:

Bash

OCP.exe -h
OCP.exe --help
OCP.exe help
