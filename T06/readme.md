## T06: Fonaments del servei DNS

Com a membres de l’equip tècnic d’EverPia, es presenta un nou repte: una auditoria completa del servei DNS per al client **DigiCore**, una empresa de màrqueting digital que experimenta errors de connectivitat en algunes de les seves aplicacions.

L’objectiu és comprendre a fons el funcionament del DNS, formar el personal tècnic del client i disposar d’eines de diagnosi que permetin detectar i resoldre incidències de manera eficient.

---

### 🎓 Fase Teòrica: Sessió formativa   

> Documentació detallada disponible a: [Fase 1](./fase1.md)
> Video disponible a: [Video](https://docs.google.com/videos/d/1_QUGD9TEVpigRI_5GcYRTMk0pz4j4arkY4Q5oIzH0X0/edit?usp=sharing)

Aquesta fase consisteix en la preparació d’una **sessió formativa** adreçada al personal de DigiCore.  
L’objectiu és oferir una explicació clara i entenedora sobre com funciona el servei DNS i quins elements en determinen el rendiment i la fiabilitat.

Un cop consolidats els conceptes, s’haurà de crear una **píndola formativa en vídeo** (entre 10 i 15 minuts) que presenti els punts principals d’una manera didàctica i visual.

#### 📌 Conceptes que s’han de tractar

- **Jerarquia i estructura DNS**  
  Explicació de l’organització en arbre: *Root > TLD > Domini de segon nivell*.

- **Procés de resolució**  
  Descripció de les consultes **iteratives** i **recursives**, així com el paper dels **Root Servers** i dels **servidors autoritatius**.

- **Tipus de zones**  
  Diferenciació entre *zona directa* i *zona inversa*, i entre *zona primària* i *zona secundària*.

- **Tipus de registres DNS**  
  Descripció i funció dels registres: `A`, `CNAME`, `MX`, `NS`, `SRV`.

- **Conceptes essencials**
  - **Resposta autoritativa:** què indica i com identificar-la.  
  - **TTL (Time To Live):** com influeix en la propagació i el rendiment.  
  - **SOA (Start of Authority):** informació que conté i importància dins d’una zona.  
  - **Reenviadors DNS:** diferència entre condicionals i incondicionals.

- **Resolució local**  
  Funcionament de la resolució sense servidor DNS i ús del protocol **mDNS**.

> 🎥 El vídeo ha d’explicar tots aquests conceptes de manera senzilla, visual i breu.

---

### 🔧 Fase Pràctica: Diagnosi DNS amb CLI  

> Documentació detallada disponible a: [Fase 2](./fase2.md)

En aquesta fase es posa en pràctica tot el coneixement adquirit, mitjançant l’ús d’eines de diagnosi DNS disponibles en diferents sistemes operatius (Linux/macOS i Windows).

Per a cada eina cal:  
1. Executar les comandes indicades.  
2. Capturar la sortida obtinguda.  
3. Analitzar els resultats i extreure’n conclusions.  

> 🖥️ L’activitat es duu a terme en un equip **Zorin OS** configurat amb dues interfícies de xarxa: **NAT** i **pont**, amb la IP assignada segons les indicacions dels responsables.

#### 🧪 Eines i proves incloses

##### A. Diagnosi avançada amb `dig` (Linux / macOS)
Execució de consultes DNS avançades i anàlisi detallada de les respostes.

##### Comprovació de resolució amb `nslookup` (Multiplataforma)
Verificació i contrast de resultats de resolució de noms en diferents entorns.

##### Resolucions locals
Comprovació de mecanismes de resolució sense servidor DNS i validació del funcionament de **mDNS**.

---

[← Tornar a la pàgina del projecte](../README.md)
