# Analisis-de-victimas-de-delitos-en-Los-Angeles-2020-2024

DESCRIPCIÓN

Este proyecto realiza un análisis de las víctimas por edad, 
género y origen étnico en la ciudad de Los Ángeles, así como el tipo de delito
y lugar de comisión del hecho. El objetivo es identificar grupos vulnerables así
como predecir patrones basados en los datos históricos

ESTRUCTURA DEL PROYECTO
Project Structure
├── README.md/               # Objetivos y descripción del proyecto
├── Dashboard/               # Análisis de datos y dashboard
├── README.md                # README

REQUISITOS

Microsoft 365 - Excel Versión 2501: 11 de febrero


METODOLOGÍA

LIMPIEZA DE DATOS Y MODELADO
-Descarga de datos
-categorización de cada columna (significado de cada una)
-cambio formato hora en columna "time OCC":
	-cambiar a formato texto, 
	-añadir 2 celdas, una con comando IZQUIERDA, otra DERECHA
	-unión de formatos con concatenación &
	-Dar formato hora.
	-Fijar formato.
        -Eliminar celdas sobrantes
-Cambio formato fecha americana a europea en columnas "RPT Date", "Date OCC"
	-Separar datos en columnas
	-usar concatenación para volver a crear un formato de fecha Columnas B y C
	-dar formato personalizado de fecha dd/mm/yyyy
	-fijar formato
	-eliminar celdas sobrantes
-Concatenación de columna w 'Weapon_desc'con columnas x, y, z cuando la columna 'weapon_cd' = 114 y 115
-Alineación de celdas columnaS I:AG
-Duplicados
 -Crear columna de duplicados
 -aplicar fórmula =SI(SI.ERROR(BUSCARV([@[DR_NO]];[DR_NO];1;falso);0);1)
 -Eliminacióm de duplicados
	Recuento	1003449
	Duplicados	5890
 -Relleno de datos mal categorizados y configuración de tabla de excel

Exploratory Data Analysis (EDA)




git clone 
[cd Crime_Data_from_2020_to_Present](https://github.com/anto-rom/Analisis-de-victimas-de-delitos-en-Los-Angeles-2020-2022)
[https://drive.google.com/file/d/1UyBvMtePHfwUkU7qsnAtrp2_KG8FVDM-/view?usp=sharing ](https://drive.google.com/file/d/1UyBvMtePHfwUkU7qsnAtrp2_KG8FVDM-/view?usp=drive_link)
https://www.dropbox.com/scl/fi/03yrz5e93m7l7xg4v5cbi/Delitos-en-los-Angeles-2020-2024.xlsb-3.zip?rlkey=phq9ocskdtzjjrnbcqba49762&st=pru61zcr&dl=0 
Install dependencies:



-----------------------------------------------------------------

Columnas
DR_NO
Número de expediente

Date Rptd
Fecha en la que el delito se ha reportado en formato DD/MM/YYYY .

DATE OCC
Fecha de comisión del delito en formato DD/MM/YYYY

TIME OCC
Hora en horario de 24 horas

Crm Cd
Código del delito cometido

Crm Cd Desc
Descripción del delito cometido

Vict Age
Edad numérica de la víctima

Vict Sex

F - Female (mujer)
M - Male (hombre)
X - Unknown (desconocido)
H - Undefined in dataset website (indefinido)

Vict Descent

Orígen étnico de la víctima

A - Other Asian
B - Black
C - Chinese
D - Cambodian
F - Filipino
G - Guamanian
H - Hispanic/Latin/Mexican
I - American Indian/Alaskan Native
J - Japanese
K - Korean
L - Laotian
O - Other
P - Pacific Islander
S - Samoan
U - Hawaiian
V - Vietnamese
W - White
X - Unknown
Z - Asian Indian
Premis Cd
Código de la estructura, vehículo o localización donde se realizó el delito

Premise Desc
Descripción del código Premis Cd

Weapon Used Cd
Tipo de arma usada

Weapon Desc
Descripción del código Weapon Used Cd

📊 Resultados y Conclusiones

-Los delitos más frecuentes en los últimos años han sido cometidos hacia
varones de raza hispana entre 30 y 49 años
-Hay un predominio del uso de armas de fuego, así como un incremento de crímenes en la 
calle y hogares particulares
-Se ha reducido significativamente los delitos en el transporte público, si bien se percibe un 
incremento en los últimos 4 años
-Los delitos que predominan es el robo de vehículos o dentro de los vehículos y el asalto callejero
con contacto físico.
-Hay una reducción de los delitos de fraude, cuyo cénit tuvo lugar en 2022
