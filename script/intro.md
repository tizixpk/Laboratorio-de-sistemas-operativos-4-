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

## Operadores aritmeticos
**1. -gt: "greater than" (mayor que)**
  - Se utiliza para verificar si un número es mayor que otro.
  - Ejemplo:
```bash
if [ $a -gt $b ]; then
    echo "$a es mayor que $b"
fi
```
**2. -eq: "equal" (igual a)**
  - Se utiliza para verificar si dos números son iguales.
  - Ejemplo
```bash
if [ $a -eq $b ]; then
    echo "$a es igual a $b"
fi
```
**3. -le: "less than or equal" (menor o igual a)**
  - Se utiliza para verificar si un número es menor o igual que otro.
  - Ejemplo
```bash
if [ $a -le $b ]; then
    echo "$a es menor o igual que $b"
fi
```
## Otros Operadores Aritméticos Comunes
 - -lt: "less than" (menor que)
    - Verifica si un número es menor que otro.
    - Ejemplo
   ```bash
   if [ $a -lt $b ]; then
    echo "$a es menor que $b"
   fi
   ```
 - -ge: "greater than or equal" (mayor o igual a)
   - Verifica si un número es mayor o igual que otro.
   - Ejemplo:
   ```bash
   if [ $a -ge $b ]; then
    echo "$a es mayor o igual que $b"
   fi
   ```
- -ne: "not equal" (no igual a)
  - Verifica si dos números no son iguales.
  - Ejemplo:
  ```bash
     if [ $a -ge $b ]; then
    echo "$a es mayor o igual que $b"
   fi
  ```
## Ejemplo Completo
```bash
#!/bin/bash

echo "Ingrese el primer número:"
read num1

echo "Ingrese el segundo número:"
read num2

if [ $num1 -gt $num2 ]; then
    echo "$num1 es mayor que $num2"
elif [ $num1 -eq $num2 ]; then
    echo "$num1 es igual a $num2"
else
    echo "$num1 es menor que $num2"
fi

if [ $num1 -le 10 ]; then
    echo "$num1 es menor o igual a 10"
fi

if [ $num2 -ge 5 ]; then
    echo "$num2 es mayor o igual a 5"
fi

if [ $num1 -ne $num2 ]; then
    echo "$num1 no es igual a $num2"
fi
```  
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

**2. case**
```bash
#!/bin/bash

echo "Ingrese una opción (a, b, c):"
read opcion

case $opcion in
    a)
        echo "Opción A seleccionada."
        ;;
    b)
        echo "Opción B seleccionada."
        ;;
    c)
        echo "Opción C seleccionada."
        ;;
    *)
        echo "Opción no válida."
        ;;
esac
```
## Bucles
**1. for**
```bash
#!/bin/bash

for i in 1 2 3 4 5; do
    echo "Número: $i"
done
```
**2. while**
```bash
#!/bin/bash

contador=1

while [ $contador -le 5 ]; do
    echo "Contador: $contador"
    contador=$((contador + 1))
done
```
**3. until**
```bash
#!/bin/bash

contador=1

until [ $contador -gt 5 ]; do
    echo "Contador: $contador"
    contador=$((contador + 1))
done
```
## Concepto de Funciones en Bash
Una función en Bash es un bloque de código reutilizable que puede ser llamado en cualquier parte del script. Las funciones permiten organizar el código de manera modular y evitar la repetición de código. Pueden aceptar parámetros y devolver valores.

### Definición de una Función
Para definir una función en Bash, puedes usar la siguiente sintaxis:
```bash
function nombre_de_la_funcion {
    # Bloque de código de la función
}
```
O alternativamente:
```bash
nombre_de_la_funcion() {
    # Bloque de código de la función
}
```
... falta completar este tema
