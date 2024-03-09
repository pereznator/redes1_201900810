<h1 align="center"> PROYECTO 1 </h1>

<p align="center">
   <img src="https://img.shields.io/badge/STATUS-EN%20DESAROLLO-green">
   </p>
<h3>UNIVERSIDAD DE SAN CARLOS DE GUATEMALA

LABORATORIO DE REDES DE COMPUTADORAS 1
PRIMER SEMESTRE 2023</h3>

<h1 align="center"> MANUAL TECNICO </h1>

Se desarrollo la topología de una red para la municipalidad de Guatemala. Ellos necesitan una red donde diferentes departamentos puedan coexistir, compartiendo el mismo medio físico, esto con el fin de ahorrar costos en instalación,  además es importante que exista redundancia, esto debido a que partes críticas de la infraestructura de la municipalidad estarán en la red. 

La red propuesta contiene 4 departamentos, Contabilidad, Secretaria, Recursos Humanos(RRHH) e Informática (IT). 
Se solicitó que no exista tránsito de datos entre departamentos, los cuales están identificados por VLANS de la siguiente forma. 

* **VLANS**

| Departamento             | VLAN | ID de red         |
|----------------------    |------|-------------------|
| Contabilidad             | 14   | 192.168.14.0/24   |
| Secretaria               | 24   | 192.168.24.0/24   |
| RRHH                     | 34   | 192.168.34.0/24   |
| IT                       | 44   | 192.168.44.0/24   |


* **IPS de Computadoras**

| Nombre            |      IP        |
|-------------------|----------------|
| CONTABILIDAD 2    | 192.168.14.1   |
| CONTABILIDAD_1    | 192.168.14.2   |
| S_CONTABILIDAD    | 192.168.14.3   |
| SECRETARIA        | 192.168.24.1   |
| SECRETARIA1       | 192.168.24.2   |
| SECRETARIA2       | 192.168.24.3   |
| RRHH              | 192.168.34.1   |
| RRHH1             | 192.168.34.2   |
| RRHH2             | 192.168.34.3   |
| S_RRHH            | 192.168.34.4   | 
| IT_2              | 192.168.44.1   |
| IT_               | 192.168.44.2   |
| S_IT              | 192.168.44.3   |



## :smile:Tecnologías Utilizadas

- Packet Tracer.

## :moneybag:Presupuesto
|Item                       |   Precion Unidad    |   Cantidad   |    Valor Agregado   |    Referencia    |
|---------------------------|--------------------:|--------------|--------------------:|------------------|
|Switch 3560                |             Q455.00 |       13     |           Q5,915.00 |  [referencia](https://www.imeqmo.com/shop/tl-sf1024-switch-tp-link-tl-sf1024-v9-0-24-puertos-10-100mbps-para-rack-17554?category=42#attr=679)|
|Switch 2960                |              Q95.00 |       8      |             Q760.00 | [referencia](https://www.imeqmo.com/shop/ms105g-switch-mercusys-ms105g-5-puertos-10-100-1000mbps-rj45-19205?category=42#attr=944)|
| Cable UTP 5e              |               Q7.00 |      100     |             Q700.00 | [referencia](https://www.steren.com.gt/cable-utp-cat5e-azul.html)|
| Cable UTP crossover       |              Q19.00 |       50     |             Q950.00 | [referencia](https://www.steren.com.gt/cable-ethernet-utp-cat-5-cruzado-crossover-de-2-1-m.html)|
| Computadora de Escritorio |            Q4607.00 |       11     |           Q50677.00 | [referencia](https://www.macrosistemas.com/producto/dell-optipliex-7010mff-i3-13100t8gbssd-256gb-wpro-11-espanol-3yrs/)| 
| Laptop                    |            Q4330.00 |       2      |            Q8660.00 | [referencia](https://www.macrosistemas.com/producto/hp-laptop-dy2076nr-intel-core-i5-1135g7-8gb-ram-256gb-ssd-2p0a3ua-15-6/)|
<!-- |---------------------------|---------------------|--------------|---------------------|------------------| -->
Total: Q67662.00

## ✒️ Autor

* **Alvaro Esaú Arenas** - *Desarrollador* - [Contacto](https://github.com/esau-arenas).
* **Jorge Antonio Pérez** - *Desarrollador* - [Contacto](https://github.com/pereznator).


