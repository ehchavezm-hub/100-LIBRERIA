# 100-LIBRERIA

Biblioteca personal de plugins, skills y hooks para Claude Code y otros agentes IA.

## Estructura

```
100-LIBRERIA/
├── plugins/
│   └── superpowers/        ← 15 skills del plugin Superpowers
│       ├── brainstorming.md
│       ├── systematic-debugging.md
│       └── ...
│
├── skills/                 ← Skills sueltos de terceros
│   └── find-skill.md       ← Busca el skill ideal antes de improvisar
│
└── hooks/                  ← Automatizaciones
    └── startup.md          ← Se ejecuta al iniciar sesión
```

## Uso en Claude Code

Copia la carpeta del skill que necesitas a `.claude/skills/` en tu proyecto:

```bash
cp 100-LIBRERIA/plugins/superpowers/brainstorming.md .claude/skills/
```

O agrega este repo como fuente en tu configuración de Claude Code.

## Fuentes

- **Superpowers**: [obra/superpowers](https://github.com/obra/superpowers) — MIT
- **find-skill**: [tammo1007/alyn](https://github.com/tammo1007/alyn) — MIT
