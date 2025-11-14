# Tasca 03 - Solucions d'emmagatzematge per a Garriga i Associats

## Descripció de la tasca
Un cop superada la fase de formació, aquest projecte té com a objectiu preparar-nos per afrontar el repte plantejat per un nou i important client: **el bufet d’advocats Garriga i Associats**, un dels més prestigiosos de la ciutat. El client gestiona una gran quantitat d'informació legal sensible, per la qual cosa la **integritat**, la **disponibilitat** (alta redundància) i la **facilitat de gestió** del seu emmagatzematge són crítics.

La direcció de Garriga i Associats ha requerit renovar els seus sistemes de servidors per garantir:
- Protecció contra fallades de disc.  
- Possibilitat d’ampliar l’espai sense interrupcions.  

Com a tècnics d’Everpia, el nostre objectiu és **dissenyar i documentar solucions d’emmagatzematge** tant per entorns Linux com Windows, complint amb els requisits d’**alta disponibilitat, redundància i escalabilitat**. Aquesta tasca es realitzarà com a prova de concepte amb màquines virtuals, i no amb servidors físics.

---

## Part 1: Linux - LVM amb Zorin OS

**Objectiu:** Demonstrar la utilitat del **Logical Volume Manager (LVM)** en un entorn Linux.

### Requisits d’implementació
1. **Configuració inicial**  
   - Crear un **grup de volums (VG)** i un **volum lògic (LV)** amb almenys dos discos de 10 GB simulats.  
   - Formatar i muntar automàticament el volum editant `/etc/fstab`.

2. **Alta disponibilitat**  
   - Implementar un **mirall (lvm_mirror)** per protegir la informació davant la fallada d’un disc.

3. **Instantànies (snapshots)**  
   - Afegir dos discos de 10 GB al grup de volums.  
   - Crear un volum `lvm_dades` amb el primer disc, formatar-lo i muntar-lo.  
   - Afegir arxius al volum (per exemple, imatges d’internet).  
   - Crear un **snapshot** `lv_snapshot` amb el segon disc i documentar el procés de restauració.

4. **Escalabilitat**  
   - Ampliar el volum `lv_dades` amb l’espai lliure disponible al grup de volums.

---

## Part 2: Windows - Espais d’Emmagatzematge (Storage Spaces)

**Objectiu:** Demonstrar les configuracions possibles amb **Storage Spaces** a Windows 11.

### Requisits d’implementació
1. **Configuració inicial**  
   - Crear un **Storage Pool** amb tres discos simulats de 10 GB.

2. **Estudi de configuracions**  
   - **Mirall (Mirroring):** Usar dos discos per alta disponibilitat.  
   - **Paritat (Parity):** Usar tres discos i explicar l’eficiència d’espai.  
   - **Mirall triple:** Afegir els discos necessaris per a aquesta configuració.

3. **Demostració de la gestió**  
   - Mostrar l’estat dels discos i del pool des de la consola de Windows.  
   - Simular la facilitat de manteniment i monitorització.

---

## Organització del treball

- El treball es realitzarà en grups dividits en dos equips:  
  - **Equip Linux:** Gestió amb LVM.  
  - **Equip Windows:** Gestió amb Storage Spaces.

- **Procediment:**  
  1. Cada membre prepara un guió de la tasca, consultant documentació i comandes.  
  2. Cada parella realitza la seva part de la demostració.  
  3. Tot el grup revisa la documentació generada.  
  4. Cada membre puja la seva documentació al seu repositori.

- La documentació es farà en **Markdown**, incloent imatges i explicacions, dins d’una carpeta `tasca03`.  
- L’arxiu `README.md` ha de contenir la descripció general de la tasca i enllaços als documents de Linux i Windows.

---

## Objectiu final
Preparar una proposta de solució d’emmagatzematge per al client, que pugui ser presentada en una **presentació conjunta** amb conclusions sobre la seva implementació i gestió.
