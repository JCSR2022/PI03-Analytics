## PI03-Analytics
Actividad Lab 03 de Henrry Trabajo con base de datos Accidentes Aereos y presentacion


El proyecto consiste en investigar los accidentes producidos desde inicios del siglo XX. Elaborando un informe y un
dashboard interactivo que recopile tal información. Para lo cual se tiene principalmente  el archivo 'AccidentesAviones.csv' sin embargo se concilia con información haciendo web scraping en otras páginas que tienen información relativa al tema en investigación como son :

https://www.epdata.es/datos/accidente-avion-datos-estadisticas/205?accion=2
http://www.planecrashinfo.com/database.htm
https://aviation-safety.net/database/
https://datos.bancomundial.org/indicator/IS.AIR.DPRT

Toda información obtenida pasa por un proceso de ETL a través de Python “221112_Procesamiento_datos Ver 01.ipynb” para después ser almacenada y presentada en el archivo final ‘221112_Presentacion_V01.pbix’

Las herramienta tecnológica utilizadas para este proyecto fueron Python(Pandas, pandasgui, SQLAlchemy, Matplotlib, Sklearn, geopy.geocoders, bs4-BeautifulSoup),  , MySQL y Power Bi para la visualización de la información procesada. 



#Se trabaja principalmente con los datos del archivo 'AccidentesAviones.csv' el cual es un archivo que 
tiene 5008 filas y 18 columnas con la siguiente informacion: 
       'fecha', 'HORA declarada', 'Ruta', 'OperadOR',
       'flight_no', 'route', 'ac_type', 'registration', 'cn_ln', 'all_aboard',
       'PASAJEROS A BORDO', 'crew_aboard', 'cantidad de fallecidos',
       'passenger_fatalities', 'crew_fatalities', 'ground', 'summary'

Este formato se tratara de unificar para coincidir con el de los datos disponbles en la pagina
' http://www.planecrashinfo.com/database.htm'

Date:	 Date of accident,  in the format - January 01, 2001
Time:	 Local time, in 24 hr. format unless otherwise specified
Airline/Op:	 Airline or operator of the aircraft
Flight #:	 Flight number assigned by the aircraft operator
Route:	 Complete or partial route flown prior to the accident
AC Type:	 Aircraft type
Reg:	 ICAO registration of the aircraft
cn / ln:	 Construction or serial number / Line or fuselage number
Aboard:	 Total aboard (passengers / crew)
Fatalities:	 Total fatalities aboard (passengers / crew)
Ground:	 Total killed on the ground
Summary:	 Brief description of the accident and cause if known


Los cambios se realizan en el programa "221112_Procesamiento_datos Ver 01.ipynb" 
obteniendo las tablas de datos necesarias para procesar en Power Bi y hacer un
analisis grafico de los mismos.

