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
nano NumerosImpares.sh
  #!/bin/bash
   echo "Ingrese El Primer Numero"
    read num1
     if [ $((num1 % 2)) -eq 0 ]; then
      echo "$num1 es un numero par"
        else
         echo "$num1 es impar"
           fi
chmod +x NumerosImpares.sh
./NumerosImpares.sh
```
**5. Imprimir los números del 1 al 10:**
```bash
nano Numeros.sh
  #!/bin/bash
    for i in 1 2 3 4 5 6 7 8 9 10; do
     echo "Número: $i"
       done
chmod +x Numeros.sh
./Numeros.sh
```
**6. Mostrar los archivos y directorios en el directorio actual:**
```bash
nano Archivos.sh
  #!/bin/bash
   ls
ch +x Archivos.sh
./Archivos.sh
```
**7. Leer una lista de nombres y mostrarlos uno por uno:**
```bash
nano Nombres.sh
  #!/bin/bash
    echo "Ingrese un nombre"
     read nombre1
      echo "Ingrese Otro Nombre"
       read nombre2
         echo "Ahora El 3er nombre"
          read nombre3
           echo "Hola $nombre1 $nombre2 $nombre3 espero que anden bien"
chmod +x Nombres.sh
./Nombres.sh


```
**8. Calcular el área de un rectángulo:**
```bash
nano Triangulos.sh
  #!/bin/bash
   echo "Ingresa La  Base"
     read base
      echo "Ingresa La Altura"
       read altura
         multiplicacion=$base * $altura
          division=$multiplicacion/2
            echo "El area del triangulo es $division
chmod +x Triangulos.sh
./Triangulos.sh
```
**9. Convertir grados Celsius a Fahrenheit:**
```bash

```
**10. Realizar una operación matemática con bc (calculadora de precisión arbitraria):**
```bash

```


