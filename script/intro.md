# Crear script en bash

1. **Abrir una terminal:**
   - En la mayoría de las distribuciones de Linux, puedes abrir una terminal usando el atajo de teclado `Ctrl + Alt + T` o buscando "Terminal" en el menú de aplicaciones.

2. **Crear un nuevo archivo de script:**
   - Puedes crear un archivo de script Bash usando cualquier editor de texto. Por ejemplo, para crear un archivo llamado `mi_script.sh`, puedes usar el comando `nano` o `vim`. Por ejemplo:
     ```bash
     nano mi_script.sh
     ```
     Esto abrirá el editor de texto "nano" con un archivo nuevo llamado `mi_script.sh`.

3. **Escribir el script:**
   - Ahora puedes escribir tu script Bash en el archivo. Aquí hay un ejemplo simple:
     ```bash
     #!/bin/bash

     # Este es un comentario
     echo "Hola, mundo!"
     ```

4. **Guardar y salir del editor de texto:**
   - En nano, puedes guardar el archivo presionando `Ctrl + O`, luego presionar Enter, y salir presionando `Ctrl + X`.

5. **Dar permisos de ejecución al script:**
   - Antes de poder ejecutar tu script, debes darle permisos de ejecución. Puedes hacerlo con el siguiente comando:
     ```bash
     chmod +x mi_script.sh
     ```

6. **Ejecutar el script:**
   - Ahora puedes ejecutar tu script Bash escribiendo:
     ```bash
     ./mi_script.sh
     ```

7. **Resultado:**
   - Después de ejecutar el script, deberías ver el mensaje "Hola, mundo!" impreso en la terminal.

