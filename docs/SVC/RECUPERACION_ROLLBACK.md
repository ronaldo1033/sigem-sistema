# Recuperacion y rollback

## Deshacer un commit ya compartido (recomendado)
```bash
git log --oneline --decorate -10
git revert <hash-del-commit>
git push
```
`git revert` crea un nuevo commit inverso y conserva el historial compartido.

## Recuperar un archivo de una version anterior
```bash
git log --oneline -- ruta/al/archivo
git restore --source=<hash> -- ruta/al/archivo
git diff
git add ruta/al/archivo
git commit -m "fix: recupera version anterior de archivo"
```

## Volver temporalmente a un commit para inspeccion
```bash
git switch --detach <hash>
git switch ronal-desarrollo
```

No ejecutar `git reset --hard` ni `push --force` sobre ramas compartidas como demostracion rutinaria: pueden perder trabajo de otros. Antes de cualquier recuperacion, revisar `git status` y respaldar cambios sin commit.
