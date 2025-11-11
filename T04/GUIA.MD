## T04: Serveis de directori - LDAP

### **1\. Objecte de l'Encàrrec**

L'objecte del present Plec és la instal·lació, configuració i validació d'un servei **OpenLDAP** en un entorn virtualitzat basat en Ubuntu Server. Aquest servei s'ha de configurar per actuar com a directori centralitzat d'usuaris i grups per al domini de proves **innovatechXX.test**.

---

### **2\. Requeriments d'Infraestructura Inicial**

El consultor ha de verificar la correcta configuració de la infraestructura virtual abans d'iniciar la implementació:

**R.INF.01 \-** Configuració de la màquina Server (Server Hostname).

![image1](./IMG/image1.png)

**R.INF.02 \-** Interfície de Xarxa Pública.

![image1](./IMG/image2.png)

**R.INF.03 \-** Interfície de Xarxa Privada.

![image1](./IMG/image3.png)

---

### **3\. Tasques d'Implementació i Configuració del Servidor LDAP**

La Consultora EverPia ha de complir estrictament amb les següents tasques d'instal·lació i configuració:

#### **3.1. Instal·lació i Configuració Base d'OpenLDAP**

**T.LDAP.01 \-** Instal·lació del servei OpenLDAP.

![image1](./IMG/image4.png)

**T.LDAP.02 \-** Configuració de la base de dades.

![image1](./IMG/image5.png)

**T.LDAP.03 \-** Configuració de la contrasenya d'administrador.

![image1](./IMG/image6.png)

**T.LDAP.04 \-** Creació d'Unitats Organitzatives (OU) inicials.

![image1](./IMG/image7.png)

**T.LDAP.05 \-** Validació de les Unitats Organitzatives.

![image1](./IMG/image8.png)

#### **3.2. Gestió i Administració (LAM)**

**T.LAM.01 \-** Instal·lació del Gestor d'Usuaris LDAP (LAM).

![image1](./IMG/image9.png)

**T.LAM.02 \-** Accés Remot i Configuració.

![image1](./IMG/image10.png)

**T.LAM.03 \-** Configuració per defecte.

![image1](./IMG/image11.png)

**T.LAM.04 \-** Creació de Grups.

![image1](./IMG/image12.png)

**T.LAM.05 \-** Creació d'Usuaris de Prova.

![image1](./IMG/image13.png)![image1](./IMG/image14.png)

---

### **4\. Integració de Client (Client Ubuntu Desktop)**

**T.CLI.01 \-** Instal·lació del Client.

![image1](./IMG/image15.png)

**T.CLI.02 \-** Resolució de Noms.

![image1](./IMG/image16.png)

**T.CLI.03** \- Validació de la Connectivitat LDAP. 

![image1](./IMG/image17.png)

**T.CLI.04 \-** Mòduls d'Autenticació.

![image1](./IMG/image18.png)

**![image1](./IMG/image19.png)![image1](./IMG/image20.png)![image1](./IMG/image21.png)]**

**T.CLI.05 \-** Configuració del Client.

![image1](./IMG/image22.png)

![image1](./IMG/image23.png)

![image1](./IMG/image24.png)

**T.CLI.06 \-** Comprovació del Sistema.

![image1](./IMG/image25.png)

**T.CLI.07 \-** Prova d'Accés Final.

![image1](./IMG/image26.png)

![image1](./IMG/image27.png)![image1](./IMG/image28.png)



