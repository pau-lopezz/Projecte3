## Espais d’Emmagatzematge Windows 11

### Configuració inicial:

![image1w](../IMG/image1w.png)

![image2w](../IMG/image2w.png)


---

### Efecte mirall doble: 

#### Partició del disc:

Primer de tot entrerem a “administrar espacios de almacenamiento”:

![image3w](../IMG/image3w.png)


Un cop dins crearem un espai de disc d'emmagatzematge, (entrem a la opció marcada).

![image4w](../IMG/image4w.png)


I s´obrirà aquest panell, que al que haurem de fer serà posar les característiques que volem que tingui al nostre disc.

![image5w](../IMG/image5w.png)


Un cop haguem posat totes les característiques, acabarem de crear al disc del tot, fen clic a la part marcada.

Ara ja podem veure el disc principal i veurel partit en dos particions en efecte mirall.

![image6w](../IMG/image6w.png)

#

#### Posar informacío dins del disc i eliminar 1 disc:

![image7w](../IMG/image7w.png)

![image8w](../IMG/image8w.png)


Ara tancarem la màquina virtual i eliminem un disc de la mateixa manera que abans haviem creat un.

![image9w](../IMG/image9w.png)  [image92](../IMG/image92w.png)


Ara podem veure que hi ha una partició que no funciona correctament, ja que hem eliminat un disc de la màquina virtual. Ara mirarem si s'ha guardat la informació en l´altre partició, per comprovar si l´efecte mirall s'ha creat correctament.

![image10w](../IMG/image10w.png)


En aquesta imatge es pot veure que se'ns ha guardat la informació correctament ✅:

![image11w](../IMG/image11w.png)


I ara podem afegir un altre cop al disc perquè no ens dongui cap error i estigui tot correcte.

![image12w](../IMG/image12w.png)

---

### Efecte mirall triple: 

Ara al primer que farem serà borrar el disc de paritat doble que hem fet per la part anterior. Un cop l´hem eliminitat hem d'afegir els discos necesaris fins a tenir 5:

![image13w](../IMG/image13w.png)


I haurem de agregar les unitats fins a tenir 5, per poder fer la partició de mirall triple.

![image14w](../IMG/image14w.png)


Ara haurem de crear un espai d´emmagatzematge amb els 5 discos com també em fet amb la part anterior, però amb reflejo triple.

![image15w](../IMG/image15w.png)


Amb amb aquesta imatge es pot comprovar que s´ha creat correctament.

![image16w](../IMG/image16w.png)


Ara posarem arxius dins, del disc i eliminem una de les unitats que hem afegit desde al VM, per veure que pasa.

![image17w](../IMG/image17w.png)


![image18w](../IMG/image18w.png)

En aquesta imatge es pot veure que ja em trencat una de les unitats partides.



I en aquí ja es veu que seguim tenint l'arxiu, la unica diferencia es que ha distribuït la informació de recuperació entre els 5 discos partits per eficiència.

![image19w](../IMG/image19w.png)

---
