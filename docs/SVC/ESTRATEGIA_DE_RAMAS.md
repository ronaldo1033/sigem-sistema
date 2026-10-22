# Estrategia de ramas de SIGEM

## Ramas permanentes
- `main`: version estable; integrar cambios mediante Pull Request y revisar pruebas.
- `ronal-desarrollo`: rama de integracion de Ronaldo.
- `<integrante>-desarrollo`: rama de integracion del segundo participante, usando su nombre real.

## Ramas temporales
- `feature/<tema>` para funcionalidades.
- `fix/<tema>` para correcciones.
- `docs/<tema>` para documentacion.
- `test/<tema>` para pruebas.

Crear ramas temporales desde la rama de integracion acordada, hacer commits pequenos y abrir un Pull Request. Tras fusionar, borrar la rama temporal si ya no se necesita. No crear ramas solo para aparentar actividad.

## Flujo recomendado
1. Actualizar la rama base con `git fetch origin` y `git pull`.
2. Crear una rama temporal con `git switch -c feature/nombre`.
3. Verificar con `git status` y ejecutar las pruebas pertinentes.
4. Registrar cambios con mensajes claros.
5. Publicar con `git push -u origin feature/nombre`.
6. Abrir un Pull Request hacia la rama acordada, solicitar revision y resolver observaciones.
7. Fusionar el PR; actualizar la rama local y borrar la temporal cuando corresponda.

No hacer `push --force` a ramas compartidas ni commits directamente a `main` salvo que el equipo acuerde una excepcion documentada.
