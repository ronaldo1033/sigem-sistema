# Convencion de commits y versiones

Usar mensajes breves, en imperativo y con prefijos consistentes:
- `feat:` nueva funcionalidad
- `fix:` correccion de error
- `docs:` documentacion
- `test:` pruebas
- `refactor:` reorganizacion sin cambiar comportamiento
- `build:` configuracion de construccion
- `chore:` mantenimiento

Ejemplos: `docs: documenta flujo de ramas`; `test: agrega prueba de validacion`; `fix: controla dato obligatorio`.

Crear tags solo para versiones verificadas. Ejemplo para una futura version, tras integrar y probar:

```bash
git switch main
git pull --ff-only origin main
git tag -a v1.1.0 -m "SIGEM 1.1.0"
git push origin v1.1.0
```

No mover ni reemplazar `v1.0.0` si ya fue publicado. Para corregir una version publicada, crear una nueva etiqueta.
