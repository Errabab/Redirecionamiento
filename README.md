# Redirecionamiento
## Enunciado: Genera un archivo llamado informe.txt que contenga la siguiente información:
* La fecha del sistema formateada. <!--date +'%d/%m/%Y %H:%M'-->
* El espacio en disco.  <!--df -h-->
* La memoria libre del sistema  <!--free -h-->
* Usuarios conectados en el sistemas.  <!--who-->
Hay que subir una imagen de que el script ha sido ejecutado con éxito.

# Respuestas:
## Script
'''
#!bin/bash <!--primera linea obligatoria-->
echo "Fecha del sistema formateada: $(date +'%d/%m/%Y %H:%M')"
echo "Espacio en el disco es:" 
(df -h) 
echo "Memoria libre del sistema es : "
(free -h)
echo "Los usurios conectados al sitema son:"
(who)
'''

