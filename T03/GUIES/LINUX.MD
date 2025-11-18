## GESTIÓ FLEXIBLE DE DISCOS (LVM amb Zorin OS)

### 1. Introducció:

#

### 2. Índex:
   1. Introducció:	
   2. Índex:	
   3. Configuracions Prèvies:	

#

### 3. Configuracions Prèvies:
Primer de tot haurem de crear una màquina virtual, hi posarem 2 CPUs i 8GB (ja que es una interfície gràfica) i afegirem 3 discs durs més de 10GB, un cop posat els requeriments de la màquina, la iniciem per procedir amb la instal·lació del OS b.

| Disc | Ús | Mida Recomanada |
| ----- | ----- | :---: |
| /dev/sda | Disc principal | **20 GB** |
| /dev/sdb | Primer disc per a LVM | **10 GB** |
| /dev/sdc | Per mirroring | **10 GB** |
| /dev/sdd | Per snapshots o expansió | **10 GB** |


![image1](../IMG/image1.png)

#

### 4. Detecció de discos:
Un cop hàgiu instal·lat tot el os, obrirem la terminal i introduirem la comanda ‘fdisk -l’ per comprovar que el sistema ha detectat els discos com a particions.


![image2](../IMG/image2.png)

#

### 5. Inicialització de discos:
Ara crearem els volums físics amb la comanda: ‘pvcreate’ a partir de les particions de la part anterior (sdb/sdc/sdd).

![image3](../IMG/image3.png)

Recordatori: Recomano que abans de començar a posar totes les comandes, recomano posar la comanda sudo su, per realitzar totes les comandes amb root així tots els processos seran més ràpids a la hora de realizarlos
