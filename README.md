# Redirecionamiento
## Genera un archivo llamado informe.txt que contenga la siguiente información:
  * La fecha del sistema formateada. <!--date +'%d/%m/%Y %H:%M'-->
  * El espacio en disco.  <!--df -h-->
  * La memoria libre del sistema  <!--free -h-->
  * Usuarios conectados en el sistemas.  <!--who-->
  

# Respuestas:
* Script
```
#!bin/bash <!--primera linea obligatoria-->
echo "Fecha del sistema formateada: $(date +'%d/%m/%Y %H:%M')" <!--comando para ver la fecha y la hora-->
echo "Espacio en el disco es:" 
(df -h) <!--comando para ver el espacio del disco-->
echo "Memoria libre del sistema es : "
(free -h) <!--comando para ver el espacio libre del disco-->
echo "Los usurios conectados al sitema son:"
(who) <!--comando para ver los usuarios conectados-->
```

* Resultado
![resultado](img/resultado_script.png)
