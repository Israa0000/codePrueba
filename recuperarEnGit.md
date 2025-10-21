si has borrado algo por git ya sea remotamente o localmente pero sigues teniendo la carpeta repositorio estos son los pasos.

1. Vete a la carperta y dale ``Shift + click derecho`` y abrir en terminal
2. si te sale algo como c66aaf3 HEAD@{6}: commit . que esto saldra cuando hagsa commit de algo el siguiente paso sera:
3. git checkout y c66aaf3 (o el numero que te aparezca al principio,no tiene que ser igual esto es un ejemplo)
4. git switch main
5. git cherry-pick c66aaf3
6. git log --oneline
7. git push origin main

y ya lo tendras subido a tu rama `main`

