<h1 align="center"> PROYECTO 2 </h1>

<p align="center">
   <img src="https://img.shields.io/badge/STATUS-EN%20DESAROLLO-green">
   </p>
<h3>UNIVERSIDAD DE SAN CARLOS DE GUATEMALA

LABORATORIO DE REDES DE COMPUTADORAS 1
PRIMER SEMESTRE 2023</h3>

<h1 align="center"> MANUAL TECNICO </h1>
El proyecto consistió en la implementación de redes para una empresa de venta de línea blanca y electrodomésticos, con el objetivo inicial de interconectar las sedes entre Jutiapa y la central de la ciudad capital. Se desarrolló una topología de red reducida para simular las interacciones entre los distintos componentes.

Para la sede de Jutiapa, se configuraron VLANs para cuatro departamentos distintos, cada uno con su segmentación de red. Se aplicó subnetting y se asignaron direcciones de red usando VLSM. Se configuraron interfaces virtuales para la puerta de acceso predeterminada de cada VLAN en el ESW1, se utilizó VTP para la propagación de las VLAN y RPVST para la prevención de bucles de red. Se configuró el protocolo LACP en SW2-SW3 y se estableció la comunicación entre los routers Jutiapa, J1 y J2 mediante HSRP, con IPs virtuales para la redundancia de primer salto.

Para la sede de Escuintla, se configuraron VLANs para dos departamentos, aplicando también subnetting y asignación de direcciones de red usando VLSM. Se utilizó VTP y RPVST, y se asignaron IPs a las VPCS.

Para la sede de Quiché, se aplicó conocimiento de subnetting y VLSM para determinar la máscara de subred adecuada, y se configuraron subinterfaces en el router Quiché para dar acceso a los equipos a la red de la empresa.

Para la sede de Petén, se configuraron interfaces virtuales para la puerta de acceso predeterminada de cada VLAN en el ESW2, y se aplicó subnetting y asignación de direcciones de red usando VLSM. Se utilizó VTP y RPVST, y se asignaron IPs a las VPCS.

Finalmente, se estableció el enrutamiento entre redes utilizando rutas estáticas para los routers frontera y ruteo dinámico OSPF para el Router Central hacia los demás routers, EIGRP para Sede Quiché y Petén, y RIP para Sede Jutiapa y Escuintla, asegurando la comunicación entre todos los equipos al finalizar la implementación.

## Sede Jutiapa
* **VLANS**

| Departamento         |Equipos    | VLAN | ID de red         |
|----------------------|-----------|------|-------------------|
| RRHH                 | 10        | 14   | 192.168.14.0/28   |
| Contabilidad         | 4         | 24   | 192.168.24.0/29   |
| Ventas               | 25        | 34   | 192.168.34.0/27   |
| Informatica          | 12        | 44   | 192.168.44.0/28   |


## Sede Escuintla
* **VLANS**

| Departamento         |Equipos    | VLAN | ID de red         |
|----------------------|-----------|------|-------------------|
| RRHH                 | 5         | 14   | 192.148.14.0/29   |
| Ventas               | 20        | 34   | 192.148.34.0/27   |

## Core
| ID de Red |
|-----------|
|10.0.0.0 /24|

## Sede Quiche
* **VLANS**

| Departamento         |Equipos    | VLAN | ID de red         |
|----------------------|-----------|------|-------------------|
| RRHH                 | 12        | 14   | 192.178.14.0/28   |
| Contabilidad         | 10        | 24   | 192.178.24.0/28   |
| Ventas               | 36        | 34   | 192.178.34.0/26   |
| Informatica          | 21        | 44   | 192.178.44.0/27   |

## Sede Peten
* **VLANS**

| Departamento         |Equipos    | VLAN | ID de red         |
|----------------------|-----------|------|-------------------|
| RRHH                 | 10        | 14   | 192.158.14.0/28   |
| Ventas               | 30        | 34   | 192.158.34.0/27   |
| Informatica          | 15        | 44   | 192.158.44.0/27   |

## ✒️ Autores

* **Alvaro Esaú Arenas** - *Desarrollador* - [Contacto](https://github.com/esau-arenas).
* **Jorge Antonio Pérez** - *Desarrollador* - [Contacto](https://github.com/pereznator).