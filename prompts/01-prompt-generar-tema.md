# Prompt: Generar Temari Desenvolupat d'un Tema

## Ús
Usa aquest prompt per demanar a la IA que desenvolupi en profunditat un tema del temari oficial, sempre a partir de fonts oficials de la Generalitat de Catalunya.

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

5. **Paraules clau** al final: llista de 10-15 termes tècnics fonamentals del tema.

6. **Possible pregunta de test** (1 exemple): una pregunta d'opció múltiple (4 opcions) representativa del tema, amb resposta correcta indicada i breu justificació. Prioritza preguntes sobre normativa o programes específics de Catalunya.

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
|-----------|-----|--------------------|
| ASPCAT | https://salutpublica.gencat.cat | Protocols, guies, informes, BEC, XVEC |
| Departament de Salut | https://salut.gencat.cat | Pla de Salut, normativa DOGC, carteres |
| DOGC | https://dogc.gencat.cat | Lleis, decrets i ordres vigents |
| Canalsalut | https://canalsalut.gencat.cat | Programes i recomanacions oficials |
