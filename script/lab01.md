# Ejercicios script en bash
**1. Imprimir "Hola, mundo!":**
```bash
nano fichero1.sh
   #!/bin/bash
    # Este es un comentario
       echo "Hola, mundo!"
chmod +x fichero1.sh
./fichero1.sh
```
**2. Imprimir la fecha y hora actual:**
```bash
nano HoraActual.sh
  #!/bin/bash
    echo "La hora actual es: $(date +%T)"
chmod +x HoraActual.sh
./HoraActual.sh
```
**3. Sumar dos números ingresados por el usuario:**
```bash
nano SumaDeNumeros.sh
  #!/bin/bash
    echo "Ingrese el 1 digito"
      read num1
         echo "Ingresa el 2 digito"
            read num2
             suma=$(expr $num1 + $num2)
               echo "La suma es: $suma"
 chmod +x SumaDeNumeros.sh
./SumaDeNumeros.sh
```
**4. Verificar si un número es par o impar:**
```bash

```
**5. Imprimir los números del 1 al 10:**
```bash

```
**6. Mostrar los archivos y directorios en el directorio actual:**
```bash

```
**7. Leer una lista de nombres y mostrarlos uno por uno:**
```bash

```
**8. Calcular el área de un rectángulo:**
```bash

```
**9. Convertir grados Celsius a Fahrenheit:**
```bash

```
**10. Realizar una operación matemática con bc (calculadora de precisión arbitraria):**
```bash

```


