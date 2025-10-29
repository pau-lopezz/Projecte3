# 📂 Implementació del Servei LDAP per a Entorn de Proves Innovatech

Aquest repositori recull tota la documentació i recursos necessaris per a la implementació d’un **servei de directori LDAP** per a l’entorn de proves d’**Innovatech**, una startup que vol centralitzar la gestió d’usuaris i grups. El projecte ha estat realitzat per la consultora tècnica **EverPia** i té com a objectiu principal instal·lar, configurar i validar un servei **OpenLDAP** en un entorn virtualitzat basat en **Ubuntu Server**.

A través d’aquest projecte, es garanteix:

- La **instal·lació i configuració** del servidor OpenLDAP amb les unitats organitzatives inicials (`users` i `groups`)  
- La **gestió i administració d’usuaris i grups** mitjançant **LAM (LDAP Account Manager)**  
- La **integració amb clients Ubuntu Desktop** per validar l’autenticació LDAP i la visibilitat dels usuaris  
- La documentació completa de **scripts, comandes i configuracions** per replicar i validar l’entorn de proves  

*(Nota: Substituir `XX` pel número de llista corresponent abans de l’execució.)*

---

## 🎯 Objectiu del Projecte

L’objectiu principal és implementar un directori centralitzat que permeti a Innovatech gestionar de manera eficient usuaris i grups dins del domini de proves `innovatechXX.test`. Aquest directori ha de ser accessible tant des del servidor com des dels clients Ubuntu Desktop, assegurant la coherència i l’autenticació correcta dels usuaris.

---

## 🛠️ Implementació i Configuració

El projecte inclou tres blocs principals:

### 1️⃣ Servidor LDAP
Es tracta de la **instal·lació i configuració d’OpenLDAP**, creant les unitats organitzatives inicials (`users` i `groups`), configurant la base de dades i l’administrador, i validant el directori amb `ldapsearch` i `slapcat`.

### 2️⃣ Gestió i Administració amb LAM
S’instal·la **LAM (LDAP Account Manager)** per facilitar la creació i gestió d’usuaris i grups. Es configuren grups de prova (`tech` i `manager`) i usuaris (`tech01` i `manager01`) amb les seves corresponents associacions.

### 3️⃣ Integració del Client Ubuntu Desktop
S’instal·la un client Ubuntu Desktop que es comunica amb el servidor LDAP a través de la interfície Host-Only. Es configuren la resolució de noms, els mòduls d’autenticació, i es valida que els usuaris del directori es visualitzen correctament en el sistema local. Finalment, es comprova l’accés dels usuaris i la creació automàtica de les seves carpetes personals.

---

## ✅ Acceptació

El projecte ha de ser validat i acceptat tant pel client **Innovatech** com per la consultora **EverPia**, signant el Plec de Condicions Tècniques (PCC) abans de la posada en producció de l’entorn de proves.
