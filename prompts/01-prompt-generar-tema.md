# Prompt: Generar Temari Desenvolupat d'un Tema

## Ús
Usa aquest prompt per demanar a la IA que desenvolupi en profunditat un tema del temari oficial, sempre a partir de fonts oficials de la Generalitat de Catalunya, incloent-hi els documents, informes i novetats publicades més recentment.

## Com usar-lo
1. Inicia la sessió carregant `context/00-context-opositor.md`
2. Indica quin tema vols treballar
3. Copia i enganxa el prompt següent, emplenant els camps entre []

---

## Prompt

```
Actua com a expert en salut pública i preparador d'oposicions per a la Generalitat de Catalunya.

Vull que desenvolupis el TEMA [NÚMERO] del temari oficial de les oposicions de tècnic superior de salut pública (Grup A, Subgrup A1, part específica).

Títol oficial del tema: [TÍTOL COMPLET DEL TEMA]

---

⚠️ CRITERI DE FONTS — OBLIGATORI I NO NEGOCIABLE

Tot el contingut d'aquest tema ha de provenir EXCLUSIVAMENT de fonts oficials de la Generalitat de Catalunya, seguint aquesta jerarquia:

1. Agència de Salut Pública de Catalunya (ASPCAT) — salutpublica.gencat.cat
   - Protocols, guies tècniques, informes, plans i programes de l'ASPCAT
   - Xarxa de Vigilància Epidemiològica de Catalunya (XVEC)
   - Butlletí Epidemiològic de Catalunya (BEC)

2. Departament de Salut de la Generalitat de Catalunya — salut.gencat.cat
   - Pla de Salut de Catalunya (vigent)
   - Lleis, decrets i ordres publicats al DOGC
   - Carteres de serveis i programes oficials

3. Altres portals de la Generalitat (DOGC, Canalsalut, altres departaments)

4. Normativa estatal (BOE) i comunitària (DOUE): NOMES per completar el marc normatiu quan Catalunya no disposi de normativa pròpia suficient, o quan la normativa catalana remeti explicitament a normativa estatal o europea.

Si no tens accés directe a les URLs en aquesta sessió, indica-ho explicitament i basa el contingut en el teu coneixement dels documents oficials de la Generalitat. Assenyala sempre: nom del document, organisme i any. Si hi ha dubtes sobre la vigència d'una dada, indica-ho amb un ⚠️ visible.

---

Requisits del desenvolupament:

1. **Introducció** (3-5 línies): contextualitza el tema i la seva importància en el marc de la salut pública a Catalunya.

2. **Epígrafs numerats** (tots els subtemes rellevants, cobertura completa del títol oficial):
   - Cada epígraf ha de tenir 150-300 paraules
   - Inclou definicions precises quan sigui necessari
   - Usa llistes amb vinyetes per a classificacions o enumeracions
   - Inclou taules comparatives quan sigui útil (normativa, tipus, categories)
   - **Al final de cada epígraf**: indica la font oficial de la Generalitat d'on prové la informació
     > 📎 *Font: [Nom del document]. [Organisme (ASPCAT / Departament de Salut / etc.)], [any].*

3. **Marc normatiu** (si escau): lleis, reglaments o directives comunitàries rellevants amb any d'aprovació. Indica si són normes catalanes (DOGC), estatals (BOE) o europees (DOUE).

4. **Documents de referència de la Generalitat** (secció obligatòria): llista dels documents oficials de la Generalitat de Catalunya — guies, protocols, plans, informes — en què es basa el tema. Format:
   ```
   - [Nom complet del document]. [Organisme]. [Any]. [URL si està disponible]
   ```

5. **🆕 Novetats i publicacions recents** (secció obligatòria):
   Aquesta secció és CLAU per a l'oposició, ja que moltes preguntes es basen en publicacions recents.
   Inclou tots els elements disponibles dels darrers 3-5 anys relacionats amb el tema:

   a) **Informes i estudis recents**: informes epidemiològics, enquestes de salut, estudis de prevalença o qualsevol publicació tècnica de l'ASPCAT o el Departament de Salut rellevant per al tema.

   b) **Guies i protocols actualitzats**: indica si hi ha versions noves de protocols o guies oficials, i assenyala els canvis principals respecte a versions anteriors.

   c) **Infografies i materials divulgatius**: si l'ASPCAT o el Departament de Salut han publicat infografies, fullets o materials visuals relacionats amb el tema, cita'ls i resumeix el seu contingut clau.

   d) **Novetats normatives**: nous decrets, ordres o instruccions publicades al DOGC en els darrers anys que afectin el tema.

   e) **Campanyes i programes nous**: noves iniciatives, campanyes de salut pública o programes posats en marxa recentment pel Govern relacionats amb el tema.

   Format per a cada element:
   > 🆕 *[Tipus: Informe / Guia / Infografia / Normativa / Campanya]*
   > **[Títol del document o iniciativa]**
   > [Organisme]. [Any de publicació].
   > Resum en 2-4 línies del contingut i per què és rellevant per a l'oposició.
   > URL: [si disponible]

   ⚠️ Si no tens informació actualitzada sobre novetats recents per a aquest tema, indica-ho explícitament i suggereix on buscar-les (p. ex., secció de "Publicacions" de salutpublica.gencat.cat o la web del Departament de Salut).

6. **Paraules clau**: llista de 10-15 termes tècnics fonamentals del tema, seleccionats per ser els més rellevants en un context d'oposició. Inclou acrònims i sigles quan s'usin habitualment (p. ex., XVEC, PPAC, BEC).

7. **Preguntes de test** (4 propostes): quatre preguntes d'opció múltiple (4 opcions cadascuna, 1 correcta) representatives del tema, amb resposta correcta indicada i breu justificació de per què és correcta i per què les altres opcions són incorrectes.

   **Diversifica les 4 preguntes** cobrint aspectes diferents del tema:
   - **Pregunta 1**: sobre conceptes o definicions fonamentals del tema.
   - **Pregunta 2**: sobre normativa o marc legal (preferentment normativa catalana, DOGC).
   - **Pregunta 3**: sobre un programa, protocol o guia específica de la Generalitat de Catalunya.
   - **Pregunta 4**: basada en una novetat o publicació recent identificada a la secció «Novetats i publicacions recents».

   Format per a cada pregunta:
   ```
   **Pregunta [N] — [Categoria: Concepte / Normativa / Programa / Novetat]**

   [Enunciat de la pregunta]

   a) [Opció A]
   b) [Opció B]
   c) [Opció C]
   d) [Opció D]

   **Resposta correcta: [lletra])**
   *Justificació*: [Explica per què és correcta i descarta breument les altres opcions. Cita la font oficial.]
   ```

Format: Markdown estructurat amb titulars ##, ###, llistes i taules.
Llengua: Català.
Nivell: Rigor tècnic per a opositor amb formació universitària en salut pública.
```

---

## Fitxer de sortida recomanat

Guarda el resultat a: `temari/tema-[NN]-[paraula-clau].md`

Exemple: `temari/tema-02-epidemiologia-mesures.md`

---

## Recordatori de fonts principals

| Organisme | URL | Tipus de contingut |
|-----------|-----|---------------------|
| ASPCAT | https://salutpublica.gencat.cat | Protocols, guies, informes, BEC, XVEC |
| Departament de Salut | https://salut.gencat.cat | Pla de Salut, normativa DOGC, carteres |
| DOGC | https://dogc.gencat.cat | Lleis, decrets i ordres vigents |
| Canalsalut | https://canalsalut.gencat.cat | Programes i recomanacions oficials |

## 🆕 Fonts recomanades per a novetats

| Recurs | URL | Tipus de contingut recent |
|--------|-----|---------------------------|
| Publicacions ASPCAT | https://salutpublica.gencat.cat/ca/el_departament/publicacions/ | Informes, guies, estudis, infografies |
| Novetats Departament de Salut | https://salut.gencat.cat/ca/el_departament/noticies/ | Notícies i comunicats oficials |
| BEC (Butlletí Epidemiològic de Catalunya) | https://salutpublica.gencat.cat/ca/vigilancia_salut_publica/bec/ | Dades epidemiològiques actualitzades |
| Canal Salut (notícies) | https://canalsalut.gencat.cat/ca/salut-a-z/ | Novetats per àrea temàtica |
| DOGC (cerques recents) | https://dogc.gencat.cat | Normativa publicada recentment |
