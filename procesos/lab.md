# Laboratorio: Gestión de procesos

1. **¿Qué es el PID?**
   - El PID (Identificador de Proceso) es un número único asignado a cada proceso en un sistema operativo Unix o similar. 

2. **¿Diferencia entre la opción –a y la opción –x de la orden ps?**
   - La opción `-a` muestra todos los procesos de todos los usuarios, mientras que la opción `-x` muestra procesos que no están asociados con una terminal.

3. **Investiga sobre el número NICE de un proceso. ¿Qué valores puede tomar el parámetro NICE? ¿Qué usuarios pueden cambiar este parámetro?**
   - El parámetro NICE de un proceso determina su prioridad de ejecución. Puede tomar valores en el rango de -20 a 19. Los usuarios con privilegios de superusuario (root) pueden cambiar este parámetro.

4. **Listar todos los archivos que contengan la cadena “.jpg” dentro de la estructura de directorios del sistema. Usar la orden ls y grep.**

5. **Ejecutar otra vez la orden anterior, pero esta vez con la prioridad más baja posible.**

6. **Abrir otra terminal, y mientras la orden anterior se ejecuta, mediante la orden ps listar todos los procesos asociados al terminal del usuario actual y obtener el PID del proceso ls. Con la orden renice otorgar la máxima prioridad a la orden ls. Después con la orden kill terminar el proceso de la manera “más correcta” posible.**

7. **Visualizar mediante el editor nano el archivo que contiene la información de los usuarios del sistema. Ejecutar el programa nano con la máxima prioridad posible.**

8. **En otro terminal, obtener el PID del editor nano y el PID de su proceso padre mediante la orden pstree.**

9. **Mediante la orden top establecer una prioridad normal al editor nano y después terminar el proceso del editor.**

10. **Ejecutar el navegador WEB firefox desde el terminar en segundo plano. Indicar el número de trabajo y su PID.**

11. **Listar todos los archivos terminados en .gif del sistema de directorios del sistema y almacenarlo en el archivo todoslosgif. Ejecutar esta orden en segundo plano.**

12. **Mediante la orden jobs listar todos los trabajos en segundo plano del terminal.**

### Procesos en 1º plano

13. **Mirar los procesos existentes en el sistema y lanzar un proceso que dure 600 segundos en 1º plano (p.e. sleep 600)**

14. **Matar el proceso. ¿Qué observamos? ¿Aparecen los mismos procesos que al principio?**

15. **Repetir el Ej. 13 y el 14, pero ahora sólo queremos detener el proceso (no cancelarlo). ¿Qué observamos? ¿Aparecen los mismos procesos que al principio?**

16. **¿Cómo podemos hacer para que continúe el proceso en 1º plano? ¿Se puede hacer con la orden kill?**

17. **Indicar dos maneras para que un proceso detenido continúe en 2º plano.**

18. **Lanzar un proceso en 2º plano y obtener su PID. ¿Cuál es su número de trabajo y número de proceso?**

19. **Si un proceso lanzado en 2º plano termina su ejecución, ¿seguirá apareciendo en la salida de jobs? Razona tu respuesta.**

20. **Detener y volver a recontinuar en 2º plano un proceso lanzado en 1º plano.**

