# Prompt: Generar Temari Desenvolupat d'un Tema

## Ús
Usa aquest prompt per demanar a la IA que desenvolupi en profunditat un tema del temari oficial.

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

Requisistos del desenvolupament:

1. **Introducció** (3-5 línies): contextualitza el tema i la seva importància en salut pública.

2. **Epígrafs numerats** (tots els subtemes rellevants, cobertura completa del títol oficial):
   - Cada epígraf ha de tenir 150-300 paraules
   - Inclou definicions precises quan sigui necessari
   - Usa llistes amb vinyetes per a classificacions o enumeracions
   - Inclou taules comparatives quan sigui útil (normativa, tipus, categories)

3. **Marc normatiu** (si escau): lleis, reglaments o directives comunitàries rellevants amb any d'aprovació.

4. **Context català** (si escau): menciona organismes com l'ASPCAT, l'Agència de Salut Pública de Catalunya, el Departament de Salut, etc.

5. **Paraules clau** al final: llista de 10-15 termes tècnics fonamentals del tema.

6. **Possible pregunta de test** (1 exemple): una pregunta d'opció múltiple (4 opcions) representativa del tema, amb resposta correcta indicada i breu justificació.

Format: Markdown estructurat amb titulars ##, ###, llistes i taules.
Llengua: Català.
Nivell: Rigor tècnic per a opositor amb formació universitària en salut pública.
```

---

## Fitxer de sortida recomanat

Guarda el resultat a: `temari/tema-[NN]-[paraula-clau].md`

Exemple: `temari/tema-02-epidemiologia-mesures.md`
