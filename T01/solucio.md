## Fase 1: Anàlisi i Justificació 

### Introducció i Justificació:
- Les contrasenyes fàcils o que s’utilitzen en molts llocs són perilloses perquè els hackers poden endevinar-les i entrar als comptes. Això pot fer que robin informació, entrin a altres comptes i facin mal a la reputació. Per això, és molt important cuidar bé les contrasenyes per estar segurs i protegir la privacitat.

  
- Un gestor de contrasenyes guarda de manera segura contrasenyes úniques i fortes per a cada compte, evita la reutilització i contrasenyes febles, i ofereix funcions com generadors automàtics, autenticació de doble factor i sincronització, millorant així la seguretat i la gestió a l’empresa.


### Comparativa Tècnica
|  | **KeePassX** | **Bitwarden** |
| :---- | ----- | ----- |
| **Ideal per** | Tots els que necessiten administrar moltes contrasenyes | Dissenyat per usuaris, grups i equips que necessiten protegir i compartir contrasenyes per protegir les seves dades privats empresarials. |
| **Implementació** | Entorn local | Basat en el núvol / Entorn local |
| **Sense connexió** | Accés sense connexió | Només lectura |
| **Preu** | Gratuït | Gratuït |
| **Codi Obert** |    ✅ |    ✅    |
| **2FA** |    ✅ |    ✅ |
| **E2EE** |    ✅ |    ✅ |


### Avantatges i Inconvenients
## 🔐 KeePass
Punts forts:
- Seguretat: Xifratge local amb AES-256 i ChaCha20, sense dependència de servidors externs.
- Usabilitat: Aplicació nativa per a Windows amb una interfície senzilla però antiquada.
- Continuïtat del negoci: Funciona localment sense necessitat de connexió a Internet, permetent un control total sobre les dades.


Punts febles:

-Seguretat: La configuració de l'autenticació multifactor (2FA) requereix plugins i pot ser complexa per a usuaris poc tècnics.
- Usabilitat: No disposa d'integració nativa amb navegadors ni aplicacions mòbils oficials; requereix plugins o ports no oficials.
- Continuïtat del negoci: La sincronització entre dispositius requereix configuració manual i pot ser difícil de gestionar en entorns empresarials amb múltiples usuaris o dispositius.


### 🔐 Bitwarden
Punts forts:
- Seguretat: Arquitectura de coneixement nul amb xifratge AES-256 i múltiples opcions de 2FA, incloent TOTP, YubiKey i biometria.
- Usabilitat: Aplicacions oficials per a Windows, macOS, Linux, iOS i Android, amb extensió per a navegadors, i sincronització automàtica entre dispositius.
- Continuïtat del negoci: Ofereix opcions de compartició de contrasenyes, accés d'emergència i capacitat d'autohostatge per a empreses, amb plans de subscripció assequibles.

Punts febles: 
- Seguretat: Algunes funcions avançades només disponibles en la versió de pagament.
- Usabilitat: Alguns usuaris han reportat problemes amb la interfície d'usuari en escriptoris i la integració amb formularis web complexos.
- Continuïtat del negoci: Algunes funcionalitats avançades estan disponibles només en la versió de pagament, i la dependència de servidors externs pot implicar riscos si fallen.
