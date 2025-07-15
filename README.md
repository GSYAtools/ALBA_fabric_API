# ALBA - Sistema para uso de la blockchain Hyperledger Fabric

## Descripción
En este repositorio se pretende diseñar un sistema con una API expuesta para nutrir de información la blockchain fabric. El objetivo de este proyecto es obtener métricas de sostenibilidad comparando un almacenamiento ligero en blockchain con otro pesado, apoyado por una base de datos MySQL que completará el almacenamiento de la información.

## Diseño inicial del sistema
Se presenta el siguiente diagrama de casos de uso para representar el sistema.
![system](https://github.com/user-attachments/assets/ee1ebe39-3545-4b28-aff3-1a4429f42138)

## Configuración de blockchain fabric
Para la versión inicial de este sistema se ha desplegado fabric utiliazndo docker en modo de consenso Raft debido al menor coste de recursos. En última instancia, se utilizará el modelo SmartBFT, con tolerancia a fallos bizantinos, con mayor consumo, pero con mayor seguridad.

## Configuración de la base de datos mysql
Se utiliza una base de datos local MySQL que contiene diferentes bases de datos, a saber (inicialmente): fabric_data y fabric_users
