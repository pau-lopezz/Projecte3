## T04: Serveis de directori - LDAP

### **1\. Objecte de l'Encàrrec**

L'objecte del present Plec és la instal·lació, configuració i validació d'un servei **OpenLDAP** en un entorn virtualitzat basat en Ubuntu Server. Aquest servei s'ha de configurar per actuar com a directori centralitzat d'usuaris i grups per al domini de proves **innovatechXX.test**.

### **2\. Requeriments d'Infraestructura Inicial**

El consultor ha de verificar la correcta configuració de la infraestructura virtual abans d'iniciar la implementació:

**R.INF.01 \-** Configuració de la màquina Server (Server Hostname).

!()[./image1.png]

**R.INF.02 \-** Interfície de Xarxa Pública.

![][image2]

**R.INF.03 \-** Interfície de Xarxa Privada.

![][image3]

---

### **3\. Tasques d'Implementació i Configuració del Servidor LDAP**

La Consultora EverPia ha de complir estrictament amb les següents tasques d'instal·lació i configuració:

#### **3.1. Instal·lació i Configuració Base d'OpenLDAP**

**T.LDAP.01 \-** Instal·lació del servei OpenLDAP.

![][image4]

**T.LDAP.02 \-** Configuració de la base de dades.

![][image5]

**T.LDAP.03 \-** Configuració de la contrasenya d'administrador.

![][image6]

**T.LDAP.04 \-** Creació d'Unitats Organitzatives (OU) inicials.

![][image7]

**T.LDAP.05 \-** Validació de les Unitats Organitzatives.

![][image8]

#### **3.2. Gestió i Administració (LAM)**

**T.LAM.01 \-** Instal·lació del Gestor d'Usuaris LDAP (LAM).

![][image9]

**T.LAM.02 \-** Accés Remot i Configuració.

![][image10]

**T.LAM.03 \-** Configuració per defecte.

![][image11]

**T.LAM.04 \-** Creació de Grups.

![][image12]

**T.LAM.05 \-** Creació d'Usuaris de Prova.

![][image13]![][image14]

---

### **4\. Integració de Client (Client Ubuntu Desktop)**

**T.CLI.01 \-** Instal·lació del Client.

![][image15]

**T.CLI.02 \-** Resolució de Noms.

![][image16]

**T.CLI.03** \- Validació de la Connectivitat LDAP. 

![][image17]

**T.CLI.04 \-** Mòduls d'Autenticació.

![][image18]

**![][image19]![][image20]![][image21]**

**T.CLI.05 \-** Configuració del Client.

![][image22]

![][image23]

![][image24]

**T.CLI.06 \-** Comprovació del Sistema.

![][image25]

**T.CLI.07 \-** Prova d'Accés Final.

![][image26]

![][image27]![][image28]



