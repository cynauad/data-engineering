# DATA ENGINEERING - CODERHOUSE

## Proyecto Final - Cynthia Auad

Comision 48145

### Objetivo:
Realizar un pipeline en airflow que viva en un contenedor Docker y realice las siguientes tareas:
1.   Conectarse a una API publica y extraer data en un archivo 
2.   Realizar trasnformaciones necesarias usando Pandas.
3.   Crear la tabla en Redshift y cargar la data.
4.   Enviar alertas mediante SMTP. 


### Descripcion de la API:

Conexion a la Api de [AviationStack](https://aviationstack.com) y extraccion de la base de datos en tiempo real (permite extraer 100 resultados, con el usuario gratuito)

### Observaciones:

- se agrega un .env para las credenciales, se muestra una copia con los pass con ***
- el airflow.config tambien fue editado para ocultar el smtp_password 
- la data extraida se guarda en redshfit. Se crea/actualiza en la task de cargar_data 
- se informa por mail la extraccion exitosa

### Imagenes 
#### Airflow

<a href="https://github.com/cynauad/data-engineering"><img src="https://github.com/cynauad/data-engineering/blob/main/Imgenes%20airflow%2C%20logs%2C%20xcom%2C%20mail/Airflow-Graph.jpg" style="height: 60%; width:60%;"/></a>

<a href="https://github.com/cynauad/data-engineering"><img src="https://github.com/cynauad/data-engineering/blob/main/Imgenes%20airflow%2C%20logs%2C%20xcom%2C%20mail/Airflow-Grid.jpg" style="height: 60%; width:60%;"/></a>

#### Xcom
<a href="https://github.com/cynauad/data-engineering"><img src="https://github.com/cynauad/data-engineering/blob/main/Imgenes%20airflow%2C%20logs%2C%20xcom%2C%20mail/Xcom1.jpg" style="height: 60%; width:60%;"/></a>
