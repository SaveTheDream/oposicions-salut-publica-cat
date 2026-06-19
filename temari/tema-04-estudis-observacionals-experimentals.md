# Tema 4 — Estudis observacionals: estudis de casos o controls i estudis de cohorts. Estudis experimentals

---

## Introducció

Els estudis epidemiològics observacionals i experimentals són les eines fonamentals per establir relacions causals entre exposicions i malalties i per avaluar l'eficàcia d'intervencions en salut pública. El domini del disseny, l'execució i la interpretació d'aquests estudis és essencial per al tècnic superior de salut pública, tant en la investigació de brots com en l'avaluació de programes preventius. A Catalunya, l'ASPCAT i el Departament de Salut utilitzen regularment aquests dissenys per a la vigilància epidemiològica i la generació d'evidència científica.

---

## 1. Estudis de casos i controls

### 1.1 Definició i estructura

L'estudi de **casos i controls** és un disseny observacional **retrospectiu** en el qual:

- Els **casos** són persones que presenten la malaltia o l'efecte d'interès.
- Els **controls** són persones sense la malaltia, seleccionades de la mateixa població d'origen que els casos.
- L'investigador compara la freqüència d'exposicions **passades** entre casos i controls per determinar si hi ha associació.

Esquemàticament:
```
POBLACIÓ → Casos (malaltia +)  → Exposició passada?
          → Controls (malaltia −) → Exposició passada?
```

### 1.2 Selecció de casos i controls

**Criteris per als casos:**
- Definició clara i precisa del cas (criteris diagnòstics estandarditzats).
- Preferiblement casos incidents (nous) per evitar el biaix de supervivència.
- Origen: registres hospitalaris, registres de malalties, notificació de MDO.

**Criteris per als controls:**
- Han de representar la població origen dels casos (la *base d'estudi*).
- Han de ser susceptibles de con vertir-se en casos si haguessin emmalaltit.
- Font habituals: població general, registre censal, malalts per una altra causa, veins o companys.
- **Aparellament (*matching*)**: assignar als controls les mateixes característiques que els casos en variables de confusió (edat, sexe, àrea geogràfica). Pot ser individual (1:1, 1:2, etc.) o per freqüència.

### 1.3 Mesura d'associació: l'Odds Ratio (OR)

En els estudis de casos i controls no es pot calcular directament la incidència, per la qual cosa la mesura d'associació és l'**odds ratio** (OR), també anomenada razó de momis o razó d'oportunitats:

| | Exposats | No exposats |
|---|---|---|
| **Casos** | a | b |
| **Controls** | c | d |

**OR = (a × d) / (b × c)**

- OR = 1: no hi ha associació.
- OR > 1: l'exposició s'associa amb més risc (factor de risc).
- OR < 1: l'exposició s'associa amb menys risc (factor protector).

Quant la malaltia és rara (prevalença <10%), l'OR és una bona aproximació del risc relatiu (RR).

### 1.4 Avantatges i limitacions

**Avantatges:**
- Eficients per a malalties **rares** o amb llarg període de latència.
- Ràpids i econòmics (no requereixen seguiment).
- Permeten estudiar múltiples factors d'exposició simultàniament.
- Útils per a la investigació de brots epidèmics.

**Limitacions:**
- Susceptibles a **biaix de record** (*recall bias*): els casos recorden l'exposició de manera diferent als controls.
- **Biaix de selecció** en la tria dels controls.
- No calculen la incidència directament.
- No aptes per a exposicions rares.
- Dificultat per establir la temporalitat de l'exposició.

### 1.5 Variants: cas-control imbricat i cas-cohort

- **Cas-control imbricat en una cohort** (*nested case-control*): els casos i controls es seleccionen d'una cohort prviament definida. Redueix biaixos i permet calcular la densitat d'incidència.
- **Disseny cas-cohort** (*case-cohort*): els controls es seleccionen aleatòriament de la cohort al principi de l'estudi, independentment de si desenvolupa la malaltia.

> 📎 *Font: Guia per a la investigació i el control de brots epidèmics. ASPCAT, 2021.*

---

## 2. Estudis de cohorts

### 2.1 Definició i estructura

L'estudi de **cohorts** és un disseny observacional en el qual es defineixen grups de persones segons la seva **exposició** (exposats i no exposats) i se segueixen en el temps per comparar la incidència de la malaltia o l'efecte d'interès.

Esquemàticament:
```
POBLACIÓ → Exposats     → Seguiment → Casos / No casos
          → No exposats  → Seguiment → Casos / No casos
```

### 2.2 Tipus de cohorts

| Tipus | Descripció | Quan s'usa |
|---|---|---|
| **Prospectiva** | S'identifiquen els subjectes al present i es segueixen cap al futur | Quan les dades d'exposició no estan disponibles prviament |
| **Retrospectiva (històrica)** | L'exposició i el seguiment es reconstrueixen a partir de registres del passat | Quan existeixen bons registres històrics (p. ex., historials laborals) |
| **Ambiespectiva** | Part retrospectiva + part prospectiva | Combina les avantatges de totes dues |

### 2.3 Mesures d'associació en estudis de cohorts

**Mesures d'incidència:**

| | Casos | No casos | Total |
|---|---|---|---|
| **Exposats** | a | b | a+b |
| **No exposats** | c | d | c+d |

- **Risc (proporcid d'atac)** en exposats: IE = a / (a+b)
- **Risc** en no exposats: INE = c / (c+d)
- **Risc Relatiu (RR)** = IE / INE
- **Reducció del risc absolut (RRA)** = IE − INE
- **Fracció atribuïble en exposats (FAE)** = (IE − INE) / IE
- **Fracció atribuïble poblacional (FAP)**: proporció de la malaltia en la població que s'eliminaría si s'eliminés l'exposició.

**Densitat d'incidència (taxa)**: quan el seguiment no és uniforme, s'utilitzen **persones-temps** com a denominador (p. ex., persones-any).

### 2.4 Avantatges i limitacions

**Avantatges:**
- Estableixen la **temporalitat** (l'exposició precedeix la malaltia): més robustesa causal.
- Permeten calcular la **incidència** directament (RR, taxes).
- Permeten avaluar múltiples efectes d'una mateixa exposició.
- Menys susceptibles al biaix de record.

**Limitacions:**
- Costosos i llargs per a malalties **rares** o amb llarg període de latència.
- Pèrdues de seguiment (*attrition bias* o biaix per pèrdues).
- **Biaix de l'usuari sa** (*healthy worker effect*): els treballadors d'una cohort laboral solen ser més sans que la població general.
- Canvis en l'exposició al llarg del temps.

### 2.5 Cohorts rellevants a Catalunya i Espanya

- **PREDIMED** (Prevención con Dieta Mediterrànea): cohort espanyola per estudiar la dieta mediterrània i la malaltia cardiovascular.
- **MCC-Spain**: estudi multicentric de casos i controls i cohort per a càncer colorectal i altres tumors.
- **Cohort COVID-19 Catalunya** (ASPCAT): seguiment de casos confirmats per avaluar sequèles i protecció vacunal.

> 📎 *Font: Protocol de vigilància epidemiològica. ASPCAT / Departament de Salut. Generalitat de Catalunya, 2020.*

---

## 3. Estudis experimentals

Els estudis experimentals es distingeixen dels observacionals perquè l'investigador **assigna activament** la intervenció o l'exposició als participants, la qual cosa permet controlar millor els factors de confusió i establir relacions causals més sòlides.

### 3.1 Assaig clínic aleatoritzat (ACA)

L'ACA és el disseny **gold standard** per avaluar l'eficàcia d'una intervenció sanitària (fàrmacs, vacunes, procediments, intervencions educatives).

**Característiques essencials:**

1. **Aleatorització**: assignació aleatòria dels participants al grup intervenció o al grup control, per garantir la comparabilitat dels grups i eliminar el biaix de selecció i la confusió.
 - *Aleatorització simple*: cada participant té la mateixa probabilitat d'anar a qualsevol grup.
 - *Aleatorització per blocs*: garanteix grups equilibrats en mida.
 - *Aleatorització estratificada*: primer s'estratifica per una variable important (p. ex., edat, sexe) i després s'aleatoritza.

2. **Cegament (*blinding*)**: 
 - **Simple cec**: el participant no sap quin tractament rep.
 - **Doble cec**: ni el participant ni l'investigador saben l'assignació.
 - **Triple cec**: tampoc sap l'analista de les dades.
 - **Obert (*open label*)**: tothom sap l'assignació (necessari en alguns dissenys quirurgics o d'intervenció conductual).

3. **Grup control**: pot rebre:
 - **Placebo**: tractament inert, per eliminar l'efecte placebo.
 - **Tractament actiu de referència** (*comparador actiu*): quan seria no ètic no tractar.
 - **Cap intervenció** (en assaigs d'intervenció sanitària o educativa).

4. **Anàlisi per intenció de tractar (ITT)**: tots els participants s'analitzen en el grup al qual van ser assignats, independentment de si van complir el tractament. Preserva els beneficis de l'aleatorització.

**Variants del disseny:**

| Variant | Descripció |
|---|---|
| **Assaig de superioritat** | Demostra que una intervenció és millor que el comparador |
| **Assaig d'equivalència** | Demostra que dues intervencions són clínicament equivalents |
| **Assaig de no inferioritat** | Demostra que la nova intervenció no és pitjor que l'estàndard |
| **Assaig creusat (*crossover*)** | Cada participant rep les dues intervencions en seqüència aleatòria |
| **Assaig factorial** | S'avaluen simultàniament dos o més intervencions independents |
| **Disseny adaptatiu** | Permet modificar el disseny durant l'assaig en funció de resultats intermedis |

> 📎 *Font: Agencia Española de Medicamentos y Productos Sanitarios (AEMPS). Guia de bones pràctiques clíniques (ICH E6). 2016.*

### 3.2 Assaig de camp (*field trial*)

- Intervenció aplicada a **individus sans** de la població general per prevenir una malaltia.
- Exemple clàssic: assaig de la vacuna de la **poliomielitis** (Salk, EUA, 1954), amb 1,8 milions de nens participants.
- Habitualment requereix grans mostres perquè els esdeveniments (noves malalties) són poc freqüents en individus sans.

### 3.3 Assaig comunitari o d'intervenció comunitària

- La unitat d'aleatorització i d'intervenció és la **comunitat** (barri, municipi, escola, empresa), no l'individu.
- Indicat per a intervencions que, per la seva naturalesa, s'apliquen al grup (p. ex., fluoració de l'aigua, campanyes de comunicació en salut pública, programes d'educació sanitària escolar).
- **Avantatge**: més realista per a intervencions comunitàries.
- **Limitació**: nombre redunat de comunitats disponibles; dificultat per aleatoritzar i per controlar la contaminació entre grups (efecte *spillover*).
- Exemple a Catalunya: programa de prevenció del tabaquisme en instituts d'educació secundària.

> 📎 *Font: Fonaments d’epidemiologia i metodologia de la recerca en salut pública. ASPCAT / Departament de Salut, Generalitat de Catalunya.*

---

## 4. Comparació dels principals dissenys epidemiològics

| Disseny | Direcció temporal | Mesura d'associació | Millor per a | Limitació principal |
|---|---|---|---|---|
| Casos i controls | Retrospectiu | OR | Malalties rares; investigació de brots | Biaix de record; no calcula incidència |
| Cohorts prospectives | Prospectiu | RR, taxes | Establir temporalitat; múltiples efectes | Cost i temps; pèrdues de seguiment |
| Cohorts retrospectives | Retrospectiu | RR, taxes | Exposicions laborals; bon registre històric | Qualitat de les dades històriques |
| Assaig clínic aleatoritzat | Prospectiu | RR, NNT | Eficàcia d'una intervenció | Cost; restriccions ètiques; generalització |
| Assaig comunitari | Prospectiu | RR, taxes | Intervencions poblacionals | Pocs grups; efecte *spillover* |

---

## 5. Biaixos específics dels estudis observacionals i experimentals

### 5.1 Biaixos en estudis de casos i controls

- **Biaix de record (*recall bias*)**: els casos tendeixen a recordar més les exposicions passades que els controls, especialment si aquestes són sòcioalment estigmatitzades o mèdicament rellevants.
- **Biaix de selecció dels controls**: si els controls no representen adequadament la població d'origen (p. ex., biaix de Berkson: controls hospitalaris sobrerepresenten exposicions).
- **Biaix de l'entrevistador**: si l'entrevistador coneix l'estatus cas/control, pot formular les preguntes de manera diferent.

### 5.2 Biaixos en estudis de cohorts

- **Pèrdues de seguiment diferencial**: si les pèrdues es relacionen amb l'exposició o la malaltia.
- **Biaix de l'usuari sa (*healthy worker effect*)**: habituals en cohorts ocupacionals.
- **Canvi d'exposició al llarg del temps** (*time-varying exposure*).
- **Biaix de l'efecte de l'im-migrant sa**: en estudis de població immigrada.

### 5.3 Biaixos en assaigs clínics

- **Biaix de selecció**: mala aleatorització o encobriment de la sequència (*allocation concealment* inadequat).
- **Biaix de desgast (*attrition bias*)**: pèrdues desiguals entre grups.
- **Biaix de notificació selectiva** (*reporting bias*): publicació selectiva de resultats positius.
- **Efecte Hawthorne**: els participants modifiquen el seu comportament pel sol fet de saber-se observats.

> 📎 *Font: Guia per a la lectura crítica d'articles científics en salut pública. ASPCAT / Departament de Salut, Generalitat de Catalunya.*

---

## 6. Ètica en la investigació epidemiològica

Qualsevol estudi que impliqui éssers humans ha de respectar els principis ètics fonamentals:

- **Principi de beneficència i no-maleficència**: la investigació ha de beneficiar la societat sense causar danys als participants.
- **Autonomia i consentiment informat**: els participants han de ser informats i han de consentir lliurement la seva participació.
- **Justicia i equitat**: els beneficis i els riscos han de distribuir-se de manera equitativa en la població.
- **Confidencialitat i protecció de dades**: regulada pel **RGPD (Reglament UE 2016/679)** i la Llei orgànica 3/2018 de protecció de dades.
- **Aprovació del Comitè Ètic d'Investigació (CEI)**: obligatòria per a tot estudi en humans.
- **Declaració de Helsinki** (1964, revisió 2013): principis ètics mínims per a la recerca mèdica que implica éssers humans.

> 📎 *Font: Llei 18/2009, de 22 d'octubre, de salut pública de Catalunya (DOGC). Departament de Salut, Generalitat de Catalunya.*

---

## 7. Marc normatiu

| Normativa | Àmbit | Any | Contingut principal |
|---|---|---|---|
| Llei 18/2009, de 22 d'octubre, de salut pública de Catalunya | DOGC | 2009 | Bases de la investigació epidemiològica i la vigilància a Catalunya |
| Llei 14/2007, de 3 de juliol, d'investigació biomèdica | BOE | 2007 | Regula la investigació en humans, biobancs i assaigs clínics |
| RD 1090/2015, de 4 de desembre, sobre assaigs clínics amb medicaments | BOE | 2015 | Transposa la Directiva 2001/20/CE; regula els ACA a Espanya |
| Reglament (UE) 536/2014 sobre assaigs clínics amb medicaments d'ús humà | UE | 2014 | Marco europeu harmonitzat per als assaigs clínics |
| Reglament (UE) 2016/679 (RGPD) | UE | 2016 | Protecció de dades personals en investigació |
| Llei orgànica 3/2018, de 5 de desembre, de protecció de dades personals | BOE | 2018 | Adaptació del RGPD a l'ordenament espanyol |
| Declaració de Helsinki | Internacional | 1964 (rev. 2013) | Principis ètics per a la investigació en éssers humans |
| RD 2210/1995, Xarxa Nacional de Vigilància Epidemiològica | BOE | 1995 | Marc de la vigilància epidemiològica estatal |

---

## 8. Documents de referència de la Generalitat de Catalunya

- Guia per a la investigació i el control de brots epidèmics. ASPCAT. 2021. https://salutpublica.gencat.cat
- Protocol de vigilància epidemiològica de les toxiinfeccions alimentàries. ASPCAT. 2020. https://salutpublica.gencat.cat
- Enquesta de Salut de Catalunya (ESCA) 2022. Departament de Salut / ASPCAT. 2022. https://salutpublica.gencat.cat
- Butlletí Epidemiològic de Catalunya (BEC). ASPCAT (publicació periòdica). https://salutpublica.gencat.cat/ca/vigilancia_salut_publica/bec/
- Informe d’avaluació de l’impacte de la COVID-19 sobre la salut de la població catalana. Departament de Salut. 2022. https://salut.gencat.cat

---

## 9. 🆕 Novetats i publicacions recents

> 🆕 *Normativa*
> **Reglament (UE) 536/2014 sobre assaigs clínics — Aplicació plena al portal europeu (CTIS) des de gener 2023**
> Comissió Europea. Aplicació plena: 2023.
> La posada en marxa del Clinical Trials Information System (CTIS) unifica la gestió i la publicitat dels assaigs clínics a la UE. Espanya i Catalunya s'han adaptat a la nova regulació, amb la plataforma centralitzada de registre i autorització d'ACA.
> URL: https://www.ema.europa.eu/en/human-regulatory-overview/research-and-development/clinical-trials-human-medicines

> 🆕 *Informe*
> **Informe de vigilància epidemiològica de Catalunya 2023 (XVEC)**
> ASPCAT. 2024.
> Inclou resultats d'estudis de brot (dissenys cas-control i cohort retrospectiva) aplicats a la investigació de toxiinfeccions alimentàries i malalties transmissibles. Exemple pràctic dels dissenys del Tema 4 aplicats a Catalunya.
> URL: https://salutpublica.gencat.cat/ca/vigilancia_salut_publica/

> 🆕 *Guia*
> **Guia metodològica per a la investigació de brots epidèmics. Actualització 2022**
> ASPCAT. 2022.
> Actualització que incorpora metodologia actualitzada per a estudis cas-control i cohort retrospectiva en la investigació de brots, incloent-hi plantilles de recollida de dades i anàlisi estadística bàsica amb taules 2x2.
> URL: https://salutpublica.gencat.cat

> 🆕 *Informe*
> **Resultats de la cohort de seguiment de COVID-19 a Catalunya (PISCIS)**
> ASPCAT / Consorci de Salut i Social de Catalunya. 2022–2024.
> La cohort PISCIS ha permès avaluar la protecció de les vacunes contra el SARS-CoV-2 i les seves variants en població catalana, publicant resultats de RR i d'efectivitat vacunal a partir de dades de registre administratiu i notificació MDO.
> URL: https://salutpublica.gencat.cat

> 🆕 *Normativa*
> **Llei 14/2007, de 3 de juliol, d'investigació biomèdica — Aplicació al context post-COVID**
> Ministerio de Sanidad / AEMPS. Actualizaciones 2022–2023.
> Reflexió sobre l'ús de dades de registre i big data en investigació epidemiològica, en el marc dels estudis observacionals generats durant i després de la pandèmia de COVID-19.
> URL: https://www.aemps.gob.es

⚠️ Per a les novetats més recents (2024–2026), es recomana consultar la secció «Publicacions» de https://salutpublica.gencat.cat i la secció de publicacions clíniques i epidemiològiques del Departament de Salut a https://salut.gencat.cat.

---

## 10. Paraules clau

1. **Estudi de casos i controls**
2. **Estudi de cohorts**
3. **Assaig clínic aleatoritzat (ACA)**
4. **Odds Ratio (OR)**
5. **Risc Relatiu (RR)**
6. **Aleatorització**
7. **Cegament (simple, doble, triple cec)**
8. **Biaix de record (*recall bias*)**
9. **Pèrdues de seguiment (*attrition bias*)**
10. **Fracció atribuïble**
11. **Anàlisi per intenció de tractar (ITT)**
12. **Aparellament (*matching*)**
13. **Assaig comunitari**
14. **Efecte Hawthorne**
15. **PISCIS** (cohort COVID-19 Catalunya)

---

## 11. Preguntes de test

---

**Pregunta 1 — Concepte**

En un estudi de casos i controls, quina és la mesura d'associació que s'utilitza habitualment?

a) El risc relatiu (RR), perquè es pot calcular directament la incidència en exposats i no exposats.
b) La fracció atribuïble poblacional (FAP), perquè quantifica la càrrega de malaltia.
c) L'odds ratio (OR), perquè no es pot calcular la incidència directament a partir d'un estudi de casos i controls.
d) La taxa de mortalitat estandarditzada (TME), perquè els casos i controls es seleccionen a partir de registres de mortalitat.

**Resposta correcta: c)**
*Justificació*: En els estudis de casos i controls, la selecció dels participants es basa en el seu estatus malalt/no malalt (no en l'exposició), de manera que no es pot calcular la incidència en exposats i no exposats. Per això s'utilitza l'OR = (a×d)/(b×c). Quan la malaltia és rara (<10%), l'OR aproxmo el RR. La fracció atribuïble (opció b) i la TME (opció d) no són les mesures específiques d'aquest disseny. Font: Guia per a la investigació de brots. ASPCAT, 2021.

---

**Pregunta 2 — Normativa**

Quina normativa regula els assaigs clínics amb medicaments d'ús humà a Espanya, en adaptació al marc europeu?

a) La Llei 14/2007, de 3 de juliol, d'investigació biomèdica, que regula tots els assaigs clínics.
b) El Reial Decret 1090/2015, de 4 de desembre, sobre assaigs clínics amb medicaments, que transposa la Directiva 2001/20/CE.
c) El Reglament (UE) 2016/679 (RGPD), que protegeix les dades dels participants en assaigs.
d) La Llei 18/2009, de 22 d'octubre, de salut pública de Catalunya, que regula la investigació epidemiològica autonòmica.

**Resposta correcta: b)**
*Justificació*: El RD 1090/2015 és la norma específica que regula els assaigs clínics amb medicaments a Espanya, transposant la Directiva europea i establint els requisits per a l'autorització, el seguiment i el notificació d'ACA. La Llei 14/2007 (opció a) regula la investigació biomèdica en general, però els ACA de medicaments queden regulats específicament pel RD 1090/2015. El RGPD (opció c) regula les dades, no els ACA. La Llei 18/2009 (opció d) és l'autonòmica catalana per a la salut pública. Font: RD 1090/2015. BOE.

---

**Pregunta 3 — Programa/Protocol**

La cohort PISCIS a Catalunya és un exemple de quin tipus d'estudi epidemiològic i per a què s'ha fet servir?

a) Assaig clínic aleatoritzat, per avaluar l'eficàcia de les vacunes contra la COVID-19 mitjançant l'assignació aleatòria dels participants.
b) Estudi de casos i controls, per comparar els factors d'exposició entre malalts greus de COVID-19 i controls.
c) Cohort de base poblacional (estudi de cohorts prospectiu i retrospectiu), per avaluar l'efectivitat vacunal contra el SARS-CoV-2 i les seves variants a partir de registres administratius i notificació MDO.
d) Estudi transversal, per determinar la prevalença de la infeccció pel SARS-CoV-2 en un moment determinat.

**Resposta correcta: c)**
*Justificació*: La cohort PISCIS (ASPCAT / Consorci de Salut i Social de Catalunya) és una cohort de base poblacional que ha aprofitat els registres administratius de Catalunya (vacunació, hospitalització, MDO) per avaluar l'efectivitat vacunal real (*real world evidence*) contra el SARS-CoV-2. No és un ACA (no hi ha aleatorització), ni un estudi transversal (hi ha seguiment longitudinal), ni un cas-control (la base és la cohort de vacunats i no vacunats). Font: ASPCAT / Consorci de Salut i Social de Catalunya, 2022–2024.

---

**Pregunta 4 — Novetat**

Al gener de 2023 va entrar en plena aplicació un sistema europeu unificat per a la gestió i publicitat dels assaigs clínics. De quin sistema es tracta i en quin reglament es fonamenta?

a) EudraVigilance, basat en el Reglament (CE) 726/2004, per a la farmacovigílància post-comercialització.
b) El Clinical Trials Information System (CTIS), basat en el Reglament (UE) 536/2014 sobre assaigs clínics amb medicaments d'ús humà.
c) El sistema RASFF, basat en el Reglament (CE) 178/2002, per a la següretat alimentària.
d) El portal EUDAMED, basat en el Reglament (UE) 2017/745, per als productes sanitaris.

**Resposta correcta: b)**
*Justificació*: El CTIS (Clinical Trials Information System) és el portal único europeu per a la gestió, l'autorització i la publicació dels resultats dels assaigs clínics, i va entrar en plena aplicació el 31 de gener de 2023, en base al Reglament (UE) 536/2014. EudraVigilance (opció a) és per a la farmacovigílància; RASFF (opció c) per a la seguretat alimentària; EUDAMED (opció d) per a productes sanitaris. Font: Comissió Europea / EMA, 2023.

---

*Document generat seguint el prompt `prompts/01-prompt-generar-tema.md` del repositori `oposicions-salut-publica-cat`.*
*Data de generació: juny 2026.*
