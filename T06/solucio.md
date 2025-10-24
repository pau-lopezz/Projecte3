## T06: Fonaments del servei DNS

### Fase teòrica: Sessió formativa

### 🧭 Fonaments del Servei DNS (Domain Name System)

### 1️⃣ Jerarquia i estructura del DNS
El DNS és com una gran guia telefònica d’internet: tradueix noms de domini fàcils d’entendre (com www.digicore.com) a adreces IP que els ordinadors utilitzen per comunicar-se (192.168.3.25, per exemple).
La seva estructura és jeràrquica i en forma d’arbre:

. (Root)
 
 ├── .com       (TLD - Top Level Domain)
 │     ├── digicore.com     (Domini de segon nivell)
 │           ├── www.digicore.com
 │           ├── mail.digicore.com
 │           └── ftp.digicore.com
 ├── .org
 └── .net

- Root Servers: hi ha 13 conjunts de servidors arrel al món que són el punt de partida de totes les consultes DNS.

- TLD Servers: gestionen dominis de primer nivell (.com, .org, .es, etc.).

- Servidors Autoritatius: contenen la informació definitiva sobre un domini concret (com digicore.com).

---

### 2️⃣ Procés de resolució de noms
Quan un usuari escriu www.digicore.com, el sistema DNS pot treballar de dues maneres:
🔹 Consulta iterativa
El client (normalment el resolver del sistema operatiu) demana informació pas a pas:

1. Demana al servidor DNS local: “Qui és www.digicore.com?”
2. Si no ho sap, el servidor li diu: “Pregunta a aquest servidor TLD.”
3. El client va seguint el camí fins trobar el servidor autoritatiu.

🔹 Consulta recursiva
El client demana al seu DNS recursor (normalment el del proveïdor d’internet) que s’encarregui de tot el procés.
Aquest servidor buscarà tota la cadena (Root → TLD → Autoritatiu) i retornarà la resposta final al client.

---

### 3️⃣ Tipus de zones DNS
Una zona DNS és la part de l’arbre que un servidor és responsable de gestionar.

- Zona directa: conté registres que associen noms de domini a IPs (ex: www → 192.168.3.25).
- Zona inversa: fa el contrari; associa una IP amb un nom (ex: 192.168.3.25 → www.digicore.com).

També hi ha:
- Zona primària (mestre): és la còpia editable i autoritativa dels registres.
- Zona secundària (esclava): és una còpia de lectura de la primària, que serveix per redundància i equilibri de càrrega.

---

### 4️⃣ Tipus de registres DNS més comuns

| Tipus | Funció | Exemple |
|-------|---------|----------|
| **A** | Associa un nom amb una adreça IPv4 | `www → 192.168.3.25` |
| **AAAA** | Igual que l’A, però per IPv6 | `www → 2001:db8::1` |
| **CNAME** | Alias d’un altre nom | `blog → www.digicore.com` |
| **MX** | Indica el servidor de correu del domini | `digicore.com → mail.digicore.com` |
| **NS** | Defineix quins servidors són autoritatius pel domini | `digicore.com → ns1.digicore.com` |
| **SRV** | Defineix serveis específics com SIP, LDAP, etc. | `_sip._tcp.digicore.com` |


---

### 5️⃣ Conceptes essencials
✅ Resposta autoritativa
Una resposta és autoritativa quan prové directament d’un servidor que conté la informació oficial del domini.
- Es pot identificar perquè el camp “AA” (Authoritative Answer) a la resposta DNS està actiu.
⏱️ TTL (Time To Live)
Indica quant de temps una resposta pot ser emmagatzemada en la memòria cau (cache).
 Un TTL alt redueix el trànsit DNS però fa que els canvis triguin més a propagar-se.
 Un TTL curt permet canvis ràpids, però augmenta el nombre de consultes.
🪪 SOA (Start of Authority)
És el registre base d’una zona DNS. Conté informació com:
- Nom del servidor primari
- Correu electrònic de l’administrador
- Número de sèrie (important per sincronitzar zones)
- Valors de refresh, retry, expire i minimum TTL

---

### 6️⃣ Reenviadors (Forwarders)
Un reenviador és un servidor DNS que passa les consultes que no pot resoldre a un altre servidor.
- Incondicional: totes les consultes que no pot resoldre localment es reenvien al servidor configurat.
- Condicional: només es reenvien les consultes d’un domini concret (ex: reenviar només .digicore.local al servidor intern de DigiCore).

--- 

### 7️⃣ Resolució local i mDNS
Quan no hi ha un servidor DNS, els equips poden resoldre noms localment:
- Fitxer hosts del sistema (manual).
- Protocol mDNS (Multicast DNS): usat en xarxes locals (com les d’oficina o domèstiques) per descobrir dispositius automàticament sense servidor. Exemple: printer.local, laptop.local.


Aquest protocol forma part de la tecnologia Bonjour / Zeroconf utilitzada per dispositius Apple i altres.



