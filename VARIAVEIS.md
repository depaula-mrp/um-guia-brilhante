# Variáveis e seus usos

### Utilitários

A variável abaixo se encontra na primeira linha de todos os scripts e é responsável por fazer a chamada do script mestre que contém todas as funções utilizadas no curso.
É possível acessar esse script pelo [link](https://code.earthengine.google.com/fa8f980b77fcbe151f54bd4727f7f26e), porém é recomendado ter conhecimento prévio de programação na plataforma.

```JavaScript

var utils = require('users/vieiramesquita/LAPIG-GEE:CURSO_GEE_LAPIG/UTILITARIOS')

```

### Satélites disponíveis

A variável satelite demonstrada abaixo é reponsável pela seleção do tipo de dado orbital que pode ser utilizado no curso. Para saber quais dados estão disponíveis, vá ao final da página e maximize seção chamada **"Opções de variáveis, realces e data"**

```JavaScript

var satelite = 'S2';

```

<details>
<summary> <b>Opções de variáveis, realces e data</b> </summary>
<p>

### [TRMM 3B43 V7 (GLOBAL)](https://developers.google.com/earth-engine/datasets/catalog/TRMM_3B43V7)
    var satelite = 'TRMM' 
    var realce = 'Chuva' 
    var data_inicial = '1998-01-01'
    var data_final = '2018-07-28'

### [ALOS DEM 30M (GLOBAL)](https://developers.google.com/earth-engine/datasets/catalog/JAXA_ALOS_AW3D30_V1_1)
    var satelite = 'ALOS' 
    var realce = 'ALT' 
Não necessita de data_inicial e/ou data_final

### [SRTM V4 30M (GLOBAL)](https://developers.google.com/earth-engine/datasets/catalog/USGS_SRTMGL1_003)
    var satelite = 'SRTM' 
    var realce = 'ALT' 
Não necessita de data_inicial e/ou data_final

### [MOD11A2 TEMPERATURA DE SUPERFICIE (GLOBAL)](https://developers.google.com/earth-engine/datasets/catalog/MODIS_006_MOD11A1)
    var satelite = 'MOD11' 
    var realce = 'TEMP' 
    var data_inicial = '2000-03-05'
    var data_final = '2018-07-28'

### [MOD13Q1 INDICE DE VEGETACAO (GLOBAL)](https://developers.google.com/earth-engine/datasets/catalog/MODIS_006_MOD13Q1)
    var satelite = 'MOD13' 
    var realce = 'NDVI' ou 'EVI' ou 'Agri'
    var data_inicial = '2000-02-18'
    var data_final = '2018-07-28'

### [MOD16A2 EVAPOTRANSPIRACAO (GLOBAL)](https://developers.google.com/earth-engine/datasets/catalog/MODIS_006_MOD16A2)
    var satelite = 'MOD16' 
    var realce = 'ET' ou 'PET'
    var data_inicial = '2000-01-01'
    var data_final = '2018-07-28' 

### [LANDSAT 5 TOA](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LT05_C01_T1_TOA) ou [LANDSAT 5 SR](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LT05_C01_T1_SR)
    var satelite = 'L5_TOA' ou 'L5_SR'
    var realce = 'Agri' ou 'False' ou 'True'
    var data_inicial = '1984-03-01'
    var data_final = 2012-05-05

### [LANDSAT 7 TOA](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LE07_C01_T1_TOA) ou [LANDSAT 7 SR](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LE07_C01_T1_SR)
    var satelite = 'L7_TOA' ou 'L7_SR'
    var realce = 'Agri' ou 'False' ou 'True'
    var data_inicial = '1999-01-01'
    var data_final = '2018-07-28' 

### [LANDSAT 8 TOA](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C01_T1_SR) ou [LANDSAT 8 SR](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C01_T1_SR)
    var satelite = 'L8_TOA' ou 'L8_SR'
    var realce = 'Agri' ou 'False' ou 'True'
    var data_inicial = '2013-04-11'
    var data_final = '2018-07-28' 

### [SENTINEL 1A & 1B SAR GRD](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S1_GRD) 
    var satelite = 'S1' 
    var realce = 'SAR' 
    var data_inicial = '2014-10-03'
    var data_final = '2018-07-28'

### [SENTINEL 2A & 2B TOA](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2)
    var satelite = 'S2' 
    var realce = 'Agri' ou 'False' ou 'False20' ou 'True'
    var data_inicial = '2015-06-23 '
    var data_final = '2018-07-28'

### [SENTINEL 3 OLCI](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S3_OLCI)
    var satelite = Sentinel 3: 'S3'
    var realce = 'False' ou 'True'
    var data_inicial = '2016-10-18'
    var data_final = '2018-07-28'

</p>
</details>