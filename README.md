# 📚 Preparació Oposicions — Tècnic de Salut Pública
## Generalitat de Catalunya · Grup A, Subgrup A1 · Part Específica

Eina per preparar les oposicions de tècnic superior de salut pública de la Generalitat de Catalunya, amb suport d'IA per generar temari desenvolupat i tests interactius.

---

## 🎯 Objectiu

Disposar d'un sistema estructurat per:
- **Generar temari** desenvolupat i ben organitzat per a cada tema del temari oficial
- **Generar tests** en Markdown o HTML per practicar i autoavaluar-se
- **Mantenir el context** entre sessions de treball amb IA

---

## 📁 Estructura del repositori

```
oposicions-salut-publica-cat/
├── context/
│   ├── 00-context-opositor.md         ← Perfil i preferències d'estudi (per iniciar sessió IA)
│   ├── 01-temari-complet.md           ← Tots els 50 temes del temari oficial
│   └── 02-temes-estabilitzacio.md     ← Temes que entren al concurs-oposició (Llei 20/2021)
├── prompts/
│   ├── 01-prompt-generar-tema.md      ← Prompt per desenvolupar un tema en profunditat
│   ├── 02-prompt-generar-test.md      ← Prompt per generar un test d'un tema
│   └── 03-prompt-sessio-estudi.md     ← Prompt per iniciar una sessió de treball continuada
├── temari/
│   └── .gitkeep                       ← Aquí es guardaran els temes desenvolupats (un fitxer per tema)
├── tests/
│   └── .gitkeep                       ← Aquí es guardaran els tests generats (Markdown o HTML)
├── log/
│   └── 00-log-iteracions.md           ← Registre de progrés i millores del mètode
└── README.md
```

---

## 🚀 Com usar-ho (flux de treball)

### Per generar el temari d'un tema nou:
1. **Obre una nova sessió** amb la IA (Perplexity, ChatGPT, etc.)
2. **Copia el contingut** de `context/00-context-opositor.md` com a primer missatge
3. **Copia el temari** de `context/01-temari-complet.md` (o el de `02-temes-estabilitzacio.md`)
4. **Enganxa el prompt** de `prompts/01-prompt-generar-tema.md` indicant el número de tema
5. Guarda el resultat a `temari/tema-XX-nom-curt.md`

### Per generar un test d'un tema:
1. **Obre una nova sessió** (o continua la mateixa)
2. **Assegura't que la IA té el context** (fitxer `00-context-opositor.md`)
3. **Adjunta el temari del tema** que vols testar (de la carpeta `temari/`)
4. **Enganxa el prompt** de `prompts/02-prompt-generar-test.md`
5. Guarda el resultat a `tests/test-tema-XX.md` o `tests/test-tema-XX.html`

### Per continuar treballant en una sessió llarga:
- Usa `prompts/03-prompt-sessio-estudi.md` per inicialitzar la IA amb tot el context necessari
- Documenta els temes treballats a `log/00-log-iteracions.md`

---

## 📋 Temes per l'estabilització (Llei 20/2021)

Per al concurs-oposició d'estabilització, les proves versaran **exclusivament** sobre:
**2, 3, 5, 6, 9, 10, 11, 12, 13, 15, 16, 17, 21, 25, 26, 27, 28, 29, 30, 31, 34, 35, 36, 37, 39, 43, 44, 48, 49 i 50**

Veure `context/02-temes-estabilitzacio.md` per als títols complets.

---

## ⚠️ Principis d'ús

- **Sempre verificar**: El temari generat és un punt de partida; contrasteu amb fonts oficials (Agència de Salut Pública de Catalunya, normativa vigent)
- **Iteració contínua**: Els prompts es poden millorar; documenta els canvis al log
- **Actualització normativa**: Algunes lleis o dades epidemiològiques poden haver canviat; reviseu la vigència
- **Estudi actiu**: Els tests són per autoavaluar-se, no per memoritzar respostes

---

## 🔄 Estat del projecte

- [x] Estructura inicial creada
- [x] Context i temari oficial carregats
- [x] Prompts inicials creats
- [ ] Primer tema desenvolupat i revisat
- [ ] Primer test generat i provat
- [ ] Cobertura dels 30 temes d'estabilització completada
- [ ] Revisió i ajust de prompts documentada
