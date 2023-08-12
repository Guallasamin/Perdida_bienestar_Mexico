# Instrucciones para el Código 'Perdida de bienestar'

Asegúrate de seguir cada uno de estos pasos en el orden indicado:

1. Descargar la Carpeta "Perdida de bienestar":
   - Cambia únicamente el directorio raíz donde deseas almacenar esta carpeta.

2. Descargar las Bases de Datos de la ENIGH:
   - Descarga las bases de datos correspondientes a la Encuesta Nacional de Ingresos y Gastos de los Hogares (ENIGH).
   - Coloca las bases de datos descargadas en la carpeta llamada "Bases".

3. Descargar Bases de Datos para los Años 2016 a 2020:
   - Descarga las bases de datos de las principales características de los hogares, gastos del hogar y gastos de los integrantes del hogar para los años 2016 a 2020.
   - Guarda las bases de datos descargadas en la siguiente convención de nombres de archivo:
     - Principales Características: `concentradohogarXXXX.csv` (donde XXXX es el año correspondiente)
     - Gastos del Hogar: `gastoshogarXXXX.csv`
     - Gastos de los Integrantes del Hogar: `gastospersonaXXXX.csv`

4. Descargar Bases de Datos para los Años 2012 y 2014 (Versión "Nueva Construcción"):
   - Descarga las bases de datos correspondientes a la versión "Nueva Construcción" de los años 2012 y 2014.
   - Aplica el mismo formato de nombres de archivo mencionado en el paso anterior para estas bases de datos.

5. Descargar Bases de Datos para los Años 2008 y 2010 (Versión "Nueva Construcción"):
   - Descarga las bases de datos correspondientes a la versión "Nueva Construcción" de los años 2008 y 2010.
   - Utiliza el formato de nombres de archivo mencionado previamente.

6. Descargar Bases de Datos para los Años 2002 a 2006 (Versión "Tradicional"):
   - Descarga las bases de datos correspondientes a la versión "Tradicional" de los años 2002 a 2006.
   - Al igual que en pasos anteriores, utiliza el formato de nombres de archivo mencionado para estas bases de datos.

7. Convertir Formato de Bases de Datos de Años 2002 a 2006 (DBF a CSV):
   - Las bases de datos de los años 2002 a 2006 están en formato DBF y deben ser convertidas a formato CSV.
   - Utiliza el siguiente código de ejemplo para realizar la conversión utilizando el paquete "foreign":

```R
install.packages("foreign")
library(foreign)
x <- read.dbf("concentradohogar2002.dbf")
write.csv(x, "concentradohogar2002.csv")
```

8. Ejecutar el Código "Perdida_de_bienestar.R":
   - Ejecuta el código llamado "Perdida_de_bienestar.R"".

9. Ver Resultados:
   - Los resultados generados por la ejecución del código aparecerán en la carpeta llamada "output".

Si sigues estos pasos correctamente, podrás ejecutar el código y visualizar los resultados generados en la carpeta "output".

## Contribuciones

¡Las contribuciones y sugerencias son bienvenidas! Si deseas mejorar la información o agregar más datos relevantes, por favor crea un pull request para su revisión.

## Licencia

Este proyecto está bajo la Licencia [MIT](LICENSE). Si decides utilizar la información contenida en estos documentos, te agradecemos si proporcionas el crédito correspondiente.

## Contacto

Si tienes preguntas o comentarios sobre el proyecto, no dudes en ponerte en contacto con nosotros en [guallasamin@gmail.com](mailto:guallasamin@gmail.com).

---
*Última actualización: Agosto 2023*
