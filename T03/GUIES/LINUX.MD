## GESTIÓ FLEXIBLE DE DISCOS (LVM amb Zorin OS)

### 1. Introducció:

#

### 2. Índex:
   1. Introducció:	
   2. Índex:	
   3. Configuracions Prèvies:	

#

### Configuracions Prèvies:
Primer de tot haurem de crear una màquina virtual, hi posarem 2 CPUs i 8GB (ja que es una interfície gràfica) i afegirem 3 discs durs més de 10GB, un cop posat els requeriments de la màquina, la iniciem per procedir amb la instal·lació del OS b.

| Disc | Ús | Mida Recomanada |
| ----- | ----- | :---: |
| /dev/sda | Disc principal | **20 GB** |
| /dev/sdb | Primer disc per a LVM | **10 GB** |
| /dev/sdc | Per mirroring | **10 GB** |
| /dev/sdd | Per snapshots o expansió | **10 GB** |


![image1](./IMG/image1.png)
