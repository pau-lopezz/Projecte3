# T06: Fonaments del servei DNS

## Breu descripció
Com a membres cada cop més integrats de l'equip tècnic de la consultora **EverPia**, teniu davant un nou repte.  
El vostre client, una empresa de màrqueting digital (**DigiCore**), experimenta de tant en tant errors de connectivitat a certes aplicacions.  
El seu equip tècnic creu que la causa principal podria ser una **resolució de noms (DNS) incorrecta o lenta**.

Se us ha encarregat realitzar una **auditoria teòrica i pràctica del servei DNS** per tal de formar el personal del client i oferir eines de diagnosi ràpides.

---

## Fase teòrica: Sessió formativa

Com a part d’aquesta formació, caldrà que elaboreu un **material formatiu pel personal del client**.  
Per assegurar la màxima qualitat dels continguts, els vostres directors tècnics han preparat unes sessions prèvies, per tal que tingueu un domini dels conceptes que després haureu d’explicar.

### Conceptes a explicar

#### Jerarquia i Estructura
- Explicació de l'estructura en arbre del DNS (Root → TLDs → Segon Nivell).

#### Procés de Resolució
- Com es realitza una consulta **iterativa** i una **recursiva**.  
- Què és un **servidor d'arrel (Root Server)** i un **servidor autoritatiu**.

#### Tipus de zones
- **Zona directa** i **zona inversa**.  
- **Zona primària** i **zona secundària**.

#### Tipus de Registres Clau (Records)
- Descripció i funció dels registres:
  - `A`
  - `CNAME`
  - `MX`
  - `NS`
  - `SVR`

#### Conceptes Essencials
- **Resposta Autoritativa:** què significa i com es pot identificar.  
- **Time To Live (TTL):** la seva funció i impacte en la propagació i el rendiment.  
- **Start of Authority (SOA):** informació essencial que conté i la seva importància.  
- **Reenviadors:** condicionals i incondicionals.  
- **Resolució local:** mecanismes de resolució sense servidor entre equips clients (protocol **mDNS**).

---

### Activitat de la fase teòrica
Un cop domineu aquests conceptes, caldrà preparar una **píndola formativa en vídeo (10–15 minuts)** que expliqui de forma breu però clara tots aquests punts.

---

## Fase pràctica: Diagnosi de Noms (Auditoria amb CLI)

Heu de demostrar l'ús de les principals **utilitats de diagnosi DNS** en diferents sistemes operatius utilitzats pel client (**Linux/macOS i Windows**).  

Per a cada eina, executeu les comandes indicades i **captureu/analitzeu els resultats**.

> 🖥️ Per a aquesta demostració, caldrà usar un equip **Zorin** amb dues interfícies:
> - Primera en **NAT**
> - Segona en **adaptador pont**, amb IP correctament configurada segons indicacions dels responsables.

---

### A. Diagnosi Avançada amb `dig` (Linux / macOS)

#### Comanda 1: Consulta Bàsica de Registre A
```bash
dig xtec.cat A

