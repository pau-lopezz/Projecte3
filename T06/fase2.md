## T06: Fonaments del servei DNS

### Fase teòrica: Fase Pràctica: Diagnosi de Noms (Auditoria amb CLI)
Heu de demostrar l'ús de les principals utilitats de diagnosi DNS en els diferents sistemes operatius que utilitza el client (Linux/macOS i Windows).

Per a cada eina, executeu les comandes indicades a continuació contra el domini que s’indiqui explícitament i captureu/analitzeu els resultats.

Per fer aquest demostració, caldrà usar un equip Zorin amb dues interfícies, la primera en NAT i la segona en adaptador pont amb la IP correctament configurada segons indicacions dels vostres responsables.

![img1](./IMG/img1.png)

---

### A. Diagnosi Avançada amb dig (Linux / macOS)
- Comanda 1: Consulta Bàsica de Registre A
  - Executa dig xtec.cat A
![img2](./IMG/img2.png)
  - Anàlisi: Identifica la IP de resposta, el valor TTL i el servidor que ha respost a la consulta.
    ```
    **IP de resposta (A record associat a xtec.cat):**
    83.247.151.214

    **TTL indicat al camp “ANSWER SECTION”:**
    3548 segons

    **Servidor que ha respost (veure “SERVER:” al final de la sortida):**
    127.0.0.53#53 (UDP) — servidor local (systemd-resolved)
