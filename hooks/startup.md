# Startup Hook

Hook que se ejecuta automáticamente al iniciar cada sesión de Claude Code.

## Comando

```
startup|clear|compact
```

## Configuración en Claude Code

En `.claude/settings.json` de tu proyecto:

```json
{
  "hooks": {
    "sessionStart": "startup|clear|compact"
  }
}
```

## Qué hace

- `startup` — Carga el contexto inicial de la sesión
- `clear` — Limpia mensajes anteriores del contexto
- `compact` — Comprime el contexto para optimizar tokens
