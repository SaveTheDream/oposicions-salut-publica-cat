# Tema 2 — Mesures de freqüència, associació i impacte en epidemiologia

> **Síntesi orientada a examen** | Fonts: ASPCAT, manuals d'epidemiologia referenciats per l'ASPCAT
> ⚠️ Present en TOTS els TC i en TOTS els SP: càlcul i interpretació de RR, RA, taxes d'atac, prevalença i incidència.

---

## 1. Mesures de freqüència

### 1.1 Incidència

Mesura la **freqüència de casos nous** d'una malaltia en una població durant un període de temps.

**Incidència acumulada (IA)**
$$IA = \frac{\text{Casos nous durant el període}}{\text{Població en risc a l'inici del període}}$$
- Expressada com a proporció (0–1) o per 100, 1.000, 100.000 habitants
- Unitat: adimensional (proporció) o per unitat de població

**Taxa d'incidència o densitat d'incidència (TI)**
$$TI = \frac{\text{Casos nous durant el període}}{\text{Suma de temps a risc de cada individu (persones-temps)}}$$
- El denominador és el **sumatori del temps que cada individu ha estat en risc** (persones-any, persones-mes)
- Unitat: casos per persones-temps (p.ex. 5 casos/1.000 persones-any)

> ⚠️ **Clau d'examen (819)**: La **taxa d'incidència** (densitat d'incidència) és la mesura que té en el denominador el **sumatori del temps a risc de cada individu expressat en persones-temps**. La incidència acumulada té en el denominador la **població en risc a l'inici**.

### 1.2 Prevalença

$$P = \frac{\text{Casos existents (nous + antics) en un moment o període}}{\text{Població total en aquell moment}}$$

- **Prevalença puntual**: en un moment concret ("fotografia")
- **Prevalença de període**: en un interval de temps
- La prevalença **NO és una mesura d'associació** ni d'impacte: és una mesura de **freqüència**

> ⚠️ **Clau d'examen (819)**: La prevalença és una mesura de **freqüència**, NO d'associació. Les mesures d'associació són el RR, la OR i el RA.

### 1.3 Relació incidència-prevalença

$$P \approx TI \times \text{durada mitjana de la malaltia}$$

Una malaltia d'alta incidència però curta durada pot tenir baixa prevalença (grip).
Una malaltia d'incidència moderada però llarga durada pot tenir alta prevalença (diabetis).

---

## 2. Mesures d'associació

### 2.1 Risc Relatiu (RR)

$$RR = \frac{\text{Incidència en exposats}}{\text{Incidència en no exposats}} = \frac{I_e}{I_{ne}}$$

| Valor RR | Interpretació |
|---|---|
| RR = 1 | No associació |
| RR > 1 | L'exposició augmenta el risc (factor de risc) |
| RR < 1 | L'exposició disminueix el risc (factor protector) |

- S'utilitza en estudis de **cohorts** i **assaigs clínics**
- Per ser estadísticament significatiu, l'interval de confiança al 95% **no ha d'incloure el valor 1**

### 2.2 Odds Ratio (OR) o Oportunitat Relativa

$$OR = \frac{a/c}{b/d} = \frac{a \times d}{b \times c}$$

- On a, b, c, d són les cel·les de la taula 2×2
- S'utilitza en estudis de **casos i controls**
- Quan la malaltia és rara, l'OR ≈ RR

---

## 3. Mesures d'impacte

### 3.1 Risc Atribuïble (RA) o diferència de riscos

$$RA = I_e - I_{ne}$$

- Quantifica l'**excés de risc** en els exposats atribuïble a l'exposició
- Exemple: si la taxa de malaltia cardiovascular (MCV) en fumadors és 655/100.000 i en no fumadors 422/100.000, el RA = 233/100.000

> ⚠️ **Clau d'examen (846, 631)**: Si la taxa en fumadors és 655/100.000 i en no fumadors 422/100.000, el nombre de morts per MCV **atribuïbles al tabac** és **233/100.000** (RA = 655 − 422 = 233).

### 3.2 Risc Atribuïble Poblacional (RAP)

$$RAP = I_{total} - I_{ne}$$

Quantifica la reducció de la incidència que s'obtindria si s'eliminés l'exposició en tota la població.

### 3.3 Taxa d'Atac (TA) — específica per brots TIA

$$TA = \frac{\text{Malalts entre els exposats a l'aliment}}{\text{Total exposats a l'aliment}} \times 100$$

**Taxa d'Atac Global (TAG)**:
$$TAG = \frac{\text{Total malalts}}{\text{Total exposats (comensals)}} \times 100$$

> ⚠️ **Clau d'examen (631 SP)**: En un brot TIA amb 76 malalts de 100 comensals, la TAG = 76/100 = **76%**.

---

## 4. Taula 2×2 i càlcul de mesures en brots TIA

|  | Malalts | Sans | Total |
|---|---|---|---|
| **Exposats a l'aliment** | a | b | a+b |
| **No exposats** | c | d | c+d |

- TA exposats = a/(a+b)
- TA no exposats = c/(c+d)
- RR = [a/(a+b)] / [c/(c+d)]

**Interpretació del RR en brots TIA:**
- RR > 1 amb IC 95% que no inclou 1 i valor-p < 0,05 → l'aliment és **sospitós**
- Com més alt és el RR, més probable que l'aliment sigui l'implicat
- Cal considerar **conjuntament** el RR, la taxa d'atac i la plausibilitat biològica

> ⚠️ **Clau d'examen (846 SP, 631 SP, 619 SP, 819 SP)**: L'aliment implicat és el que té el **RR més alt** amb interval de confiança que **no inclou l'1** i valor-p significatiu.

---

## 5. Resum: classificació de les mesures

| Tipus de mesura | Mesures incloses |
|---|---|
| **Mesures de freqüència** | Prevalença, incidència acumulada, taxa d'incidència |
| **Mesures d'associació** | RR, OR |
| **Mesures d'impacte** | Risc atribuïble (RA), RAP, fracció atribuïble |

> 📄 **Fonts**: *Epidemiologia bàsica i vigilància de la salut*. Departament de Salut, Generalitat de Catalunya. / Protocols de vigilància epidemiològica, ASPCAT.
