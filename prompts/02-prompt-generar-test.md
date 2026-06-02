# Prompt: Generar Test Interactiu d'un Tema

## Ús
Usa aquest prompt per generar un test de preguntes tipus test a partir del temari desenvolupat d'un tema, calibrat a l'estil i dificultat dels testos reals d'oposicions.

## Com usar-lo
1. Assegura't que la IA té el context (`context/00-context-opositor.md`)
2. Adjunta o enganxa el temari del tema en qüestió (de la carpeta `temari/`)
3. Indica si vols que la IA consulti l'anàlisi de testos reals (`context/03-analisi-testos-reals.md`)
4. Indica el format de sortida desitjat: **Markdown** o **HTML interactiu**
5. Copia i enganxa el prompt següent

---

## Prompt (format Markdown)

```
Actua com a preparador expert d'oposicions de tècnic superior de salut pública de la Generalitat de Catalunya.

A partir del temari del Tema [NÚMERO] — [TÍTOL] que t'he proporcionat, genera un test de preguntes tipus test per preparar les oposicions.

---

⚠️ CRITERI DE FONTS — OBLIGATORI
El contingut de les preguntes ha de provenir exclusivament de fonts oficials de la Generalitat de Catalunya (ASPCAT, Departament de Salut, DOGC), tal com s'especifica al fitxer `context/00-context-opositor.md`. La normativa estatal o europea s'inclou només quan el temari català la referencia directament.

---

⚠️ ESTIL DE LES PREGUNTES — OBLIGATORI
Els testos han de replicar l'estil dels testos reals de la convocatoria 833 (procés 846, abril 2025), analitzats al fitxer `context/03-analisi-testos-reals.md`. Això implica:

1. **Preguntes molt específiques i factuals**: articles concrets de normativa, annexos, xifres, temperatures, terminis, percentatges.
2. **Preguntes sobre programes catalans concrets**: nom exacte, població diana, organisme responsable, període.
3. **Preguntes de concepte amb negació**: "Quina de les afirmacions següents NO és certa / és falsa / és incorrecta?"
4. **Distractors plausibles**: les opcions incorrectes han de semblar versemblants (canviar dates, xifres, organismes o conceptes similars).
5. **No repetir ni reformular preguntes** que ja apareguin al fitxer `context/03-analisi-testos-reals.md`.

---

Requisistos del test:
- **20 preguntes** d'opció múltiple (4 opcions: a, b, c, d)
- **1 sola resposta correcta** per pregunta
- Preguntes distribuïdes proporcionalment entre els epígrafs del tema
- Nivell de dificultat: **intermedi-alt** (adequat per a oposicions grup A)
- Inclou preguntes de:
  - Normativa concreta (articles, annexos, valors, terminis)
  - Programes i plans catalans de l'ASPCAT o Departament de Salut
  - Conceptes i definicions tècniques
  - Aplicació pràctica o cas concret

Format de sortida: **Markdown**

Estructura per a cada pregunta:
```
**Pregunta X.** [Enunciat de la pregunta]

a) [Opció A]
b) [Opció B]
c) [Opció C]
d) [Opció D]

<details>
<summary>Resposta correcta</summary>

**Resposta: [lletra]** — [justificació breu de 2-3 línies, incloent la font oficial]
</details>
```

Llengua: Català.
```

---

## Prompt (format HTML interactiu)

```
Actua com a preparador expert d'oposicions de tècnic superior de salut pública de la Generalitat de Catalunya.

A partir del temari del Tema [NÚMERO] — [TÍTOL] que t'he proporcionat, genera un test interactiu en HTML.

---

⚠️ CRITERI DE FONTS — OBLIGATORI
El contingut de les preguntes ha de provenir exclusivament de fonts oficials de la Generalitat de Catalunya (ASPCAT, Departament de Salut, DOGC). La normativa estatal o europea s'inclou només quan el temari català la referencia directament.

---

⚠️ ESTIL DE LES PREGUNTES — OBLIGATORI
Els testos han de replicar l'estil dels testos reals de la convocatoria 833 (procés 846, abril 2025), analitzats al fitxer `context/03-analisi-testos-reals.md`:

1. Preguntes factuals i específiques (articles, xifres, terminis)
2. Preguntes sobre programes catalans concrets de l'ASPCAT
3. ús freqüent de la negació ("NO és", "és falsa")
4. Distractors plausibles (no absurds)
5. No repetir ni reformular preguntes del fitxer `context/03-analisi-testos-reals.md`

---

Requisistos del test:
- **20 preguntes** d'opció múltiple (4 opcions: a, b, c, d), 1 correcta
- Nivell intermedi-alt (grup A)
- Preguntes cobreixen tots els epígrafs del tema

Requisistos tècnics de l'HTML:
- Fitxer HTML autocontingut (tot en un sol fitxer: HTML + CSS + JS inline)
- Disseny net i professional, responsive
- Funcionalitat:
  - L'usuari selecciona una opció i confirma
  - Mostra si és correcta o incorrecta amb la justificació i la font oficial
  - Comptador de preguntes i puntuació al final
  - Botó per reiniciar el test
  - Indicador de " has vist X de 20 preguntes"
- Colors: resposta correcta en verd, incorrecta en vermell
- Inclou el número i títol del tema a la capçalera
- Sense dependències externes (cap CDN, tot inline)

Llengua del test: Català.
```

---

## Prompt (supòsit pràctic HTML)

```
Actua com a preparador expert d'oposicions de tècnic superior de salut pública de la Generalitat de Catalunya.

Genera un supòsit pràctic tipus test en HTML, seguint el model dels supòsits reals de la convocatoria 833 (procés 846, abril 2025).

---

⚠️ ESTIL OBLIGATORI — Model de referencia:
- El candidat és un tècnic/a de nova incorporació en rotació per un SSP, SPS i SVE
- El supòsit té 3-5 situacions professionals amb 5 preguntes cadascuna
- Cada situació és un cas real (brot, inspecció, programa, alerta) que el tècnic ha d'afrontar
- Les preguntes combinen càlculs (RR, RAe, TAe), decisió professional i aplicació de normativa concreta
- Les situacions poden ser transversals (tocar més d'un tema del temari)
- No repetir ni reformular les situacions del fitxer `context/03-analisi-testos-reals.md`

Temes del temari que vull incloure al supòsit: [LLISTA DE TEMES]

---

Requisistos tècnics de l'HTML:
- Fitxer HTML autocontingut (HTML + CSS + JS inline)
- Disseny net i professional, responsive
- Presenta el text introductori de cada situació amb claredat
- Funcionalitat:
  - L'usuari llegeix la situació i respon les preguntes una a una
  - Confirmació de resposta amb feedback immediat i justificació
  - Puntuació final per situació i global
  - Botó per reiniciar
- Colors: resposta correcta en verd, incorrecta en vermell
- Sense dependències externes

Llengua: Català.
```

---

## Fitxer de sortida recomanat

Guarda el resultat a:
- Markdown: `tests/test-tema-[NN].md`
- HTML test coneixements: `tests/test-tema-[NN].html`
- HTML supòsit: `tests/suposit-[NOM-CURT].html`

---

## Recordatori: què NO han de fer els tests

- ❌ No repetir preguntes del fitxer `context/03-analisi-testos-reals.md`
- ❌ No reformular les mateixes preguntes canviant només la redacció
- ❌ No fer preguntes evidentment trivials o amb distractors absurds
- ✅ Sí reutilitzar el **format i estil** dels testos reals
- ✅ Sí partir del **temari oficial** per cobrir àrees que els testos reals no han cobert
