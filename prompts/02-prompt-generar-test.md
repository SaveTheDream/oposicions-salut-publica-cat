# Prompt: Generar Test Interactiu d'un Tema

## Ús
Usa aquest prompt per generar un test de preguntes tipus test a partir del temari desenvolupat d'un tema.

## Com usar-lo
1. Assegura't que la IA té el context (`context/00-context-opositor.md`)
2. Adjunta o enganxa el temari del tema en qüestió (de la carpeta `temari/`)
3. Indica el format de sortida desitjat: **Markdown** o **HTML interactiu**
4. Copia i enganxa el prompt següent

---

## Prompt (format Markdown)

```
A partir del temari del Tema [NÚMERO] — [TÍTOL] que t'he proporcionat, genera un test de preguntes tipus test per a la preparació de les oposicions de tècnic superior de salut pública de la Generalitat de Catalunya.

Requisistos del test:
- **20 preguntes** d'opció múltiple (4 opcions: a, b, c, d)
- **1 sola resposta correcta** per pregunta
- Preguntes distribuïdes proporcionalment entre els epígrafs del tema
- Nivell de dificultat: **intermedi-alt** (adequat per a oposicions grup A)
- Inclou preguntes de:
  - Definicions i conceptes clau
  - Normativa (lleis, anys, organismes)
  - Aplicació pràctica i casos
  - Comparació entre conceptes similars

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

**Resposta: [lletra]**

[Justificació breu de 2-3 línies]
</details>
```

Llengua: Català.
```

---

## Prompt (format HTML interactiu)

```
A partir del temari del Tema [NÚMERO] — [TÍTOL] que t'he proporcionat, genera un test interactiu en HTML per a la preparació de les oposicions de tècnic superior de salut pública de la Generalitat de Catalunya.

Requisistos del test:
- **20 preguntes** d'opció múltiple (4 opcions: a, b, c, d), 1 correcta
- Nivell intermedi-alt (grup A)
- Preguntes cobreixen tots els epígrafs del tema

Requisistos tècnics de l'HTML:
- Fitxer HTML autocontingut (tot en un sol fitxer: HTML + CSS + JS inline)
- Disseny net i professional, responsive
- Funcionalitat:
  - L'usuari selecciona una opció i confirma
  - Mostra si és correcta o incorrecta, amb la justificació
  - Comptador de preguntes i puntuació al final
  - Botó per reiniciar el test
- Colors: resposta correcta en verd, incorrecta en vermell
- Sense dependències externes (cap CDN, tot inline)

Llengua del test: Català.
```

---

## Fitxer de sortida recomanat

Guarda el resultat a:
- Markdown: `tests/test-tema-[NN].md`
- HTML: `tests/test-tema-[NN].html`

Exemple: `tests/test-tema-02.md` o `tests/test-tema-02.html`
