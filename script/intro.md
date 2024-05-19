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

## Comandos basicos I/O
```bash
#!/bin/bash

# Pedir el nombre del usuario
echo "Ingrese su nombre:"
read nombre

# Pedir la edad del usuario
echo "Ingrese su edad:"
read edad

# Mostrar los datos ingresados
echo "Hola, $nombre! Tienes $edad años."

# Usar printf para mostrar los datos de manera formateada
printf "Nombre: %s\nEdad: %d\n" "$nombre" "$edad"
```
## Estructuras Condicionales
**1. if-else**
```bash
if [ condición ]; then
    # Bloque de comandos si la condición es verdadera
elif [ otra_condición ]; then
    # Bloque de comandos si la otra_condición es verdadera
else
    # Bloque de comandos si ninguna de las condiciones anteriores es verdadera
fi
```
**2. case**
```bash
case $variable in
    valor1)
        # Comandos para valor1
        ;;
    valor2)
        # Comandos para valor2
        ;;
    *)
        # Comandos para cualquier otro valor
        ;;
esac
```
## Bucles
**1. for**
```bash
for variable in lista; do
    # Bloque de comandos
done
```
**2. while**
```bash
while [ condición ]; do
    # Bloque de comandos
done
```
**3. until**
```bash
until [ condición ]; do
    # Bloque de comandos
done
```
## Ejemplos Prácticos
**1. if-else**
```bash
#!/bin/bash

echo "Ingrese un número:"
read num

if [ $num -gt 10 ]; then
    echo "El número es mayor que 10."
elif [ $num -eq 10 ]; then
    echo "El número es igual a 10."
else
    echo "El número es menor que 10."
fi
```





