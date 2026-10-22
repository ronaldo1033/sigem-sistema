# Guía de colaboración

## Flujo de trabajo

- `main`: versión integrada y estable.
- `ronal-desarrollo`: rama de trabajo de Ronaldo.
- Cada integrante debe trabajar en su propia rama, por ejemplo `nombre-desarrollo`.
- Usar commits pequeños con mensajes descriptivos.
- Integrar cambios mediante Pull Request hacia `main` después de revisar y probar.

## Convención de commits

Usar mensajes como `feat: agrega ...`, `fix: corrige ...`, `docs: actualiza ...`, `test: agrega ...` y `refactor: ...`.

## Antes de publicar

- No subir `.env`, contraseñas reales, tokens, llaves privadas ni datos personales.
- Mantener los secretos en variables de entorno.
- Ejecutar las pruebas disponibles y verificar la configuración de PostgreSQL.
