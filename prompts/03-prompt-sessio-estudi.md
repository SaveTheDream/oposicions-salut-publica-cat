# Prompt: Iniciar una Sessió de Treball Continuada

## Ús
Usa aquest prompt per inicialitzar una sessió de treball llarga en la qual vols treballar diversos temes seguits, o per reprendre el fil d'una sessió anterior.

## Com usar-lo
1. Obre una nova sessió amb la IA
2. Copia i enganxa primer el context (`context/00-context-opositor.md`)
3. Indica quins temes has treballat ja (consulta el log)
4. Copia i enganxa el prompt de sessió

---

## Prompt de sessió

```
Actua com a preparador expert d'oposicions de salut pública de la Generalitat de Catalunya.

Contexte del projecte:
- Estic preparant les oposicions de tècnic superior de salut pública (Grup A, Subgrup A1, part específica)
- Tenim un repositori GitHub estructurat amb context, prompts, temari i tests
- Les sessions de treball s'han de poder reprendre fàcilment

Estat actual de la preparació:
- Temes treballats fins ara: [LLISTA DE TEMES JA COBERTS]
- Temes pendents d'alta prioritat: [TEMES QUE VOLS FER AVUI]
- Log de la darrera sessió: [RESUM BREU DE L'ÚLTIMA SESSIÓ, O "primera sessió"]

Pla de treball per a aquesta sessió:
1. [PRIMER OBJECTIU: per exemple, "Desenvolupar el Tema 5"]
2. [SEGON OBJECTIU: per exemple, "Generar test del Tema 2 en HTML"]
3. [TERCER OBJECTIU, si escau]

Instruccions generals:
- Treballem en català
- Rigor tècnic, nivell universitari
- Quan acabem un tema o test, avisa'm per poder desar el resultat al repositori
- Si detectes inconsistències o pots millorar algun prompt, indica-m'ho

Comença pel primer objectiu. Confirma que has entès el pla de treball.
```

---

## Fitxer de sortida

Després de cada sessió, actualitza `log/00-log-iteracions.md` amb:
- Data de la sessió
- Temes treballats
- Fitxers creats
- Notes de millora
