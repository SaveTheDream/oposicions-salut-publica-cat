# Testos Reals d'Oposicions

Aquesta carpeta emmagatzema els testos i plantilles de correcció dels processos selectius anteriors de tècnic superior de salut pública (Generalitat de Catalunya).

## Estructura

```
testos-reals/
├── README.md                  ← Aquest fitxer
├── TC/                        ← Tests de coneixements (enunciats)
│   └── 03_TC_846-2.pdf
├── SP/                        ← Supòsits pràctics (enunciats)
│   └── 03_SP_846.pdf
└── PC/                        ← Plantilles de correcció
    ├── 03_TC_846_PC.pdf
    ├── 03_SP_846_PC-2.pdf
    └── respostes-846.md       ← Respostes en Markdown (consulta ràpida)
```

## Convencions de noms

| Element | Nomenclatura | Exemple |
|---------|-------------|---------|
| Test coneixements | `TC_[codi].pdf` | `TC_846-2.pdf` |
| Supòsit pràctic | `SP_[codi].pdf` | `SP_846.pdf` |
| Plantilla TC | `TC_[codi]_PC.pdf` | `TC_846_PC.pdf` |
| Plantilla SP | `SP_[codi]_PC.pdf` | `SP_846_PC-2.pdf` |

## Processos disponibles

| Conv. | Codi procés | Data | TC | SP | PC-TC | PC-SP | Anàlisi context |
|-------|------------|------|----|----|-------|-------|------------------|
| 833 | 846 | 06/04/2025 | ✅ | ✅ | ✅ | ✅ | `context/03-analisi-testos-reals.md` |

## Com afegir un nou procés

1. Puja els PDFs a les carpetes corresponents (`TC/`, `SP/`, `PC/`)
2. Afegeix una fila a la taula de processos disponibles d'aquest README
3. Afegeix un fitxer `respostes-[codi].md` a la carpeta `PC/`
4. Actualitza `context/03-analisi-testos-reals.md` amb l'anàlisi del nou procés
