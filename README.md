\# Flujo GitFlow Implementado



\##Esquema del Flujo

\* ded66d3 (develop) chore(release): preparar versión 1.0

\*   5cd2227 Merge branch 'feature/contacto' into develop

|\\

| \* 9bdf6af (feature/contacto) feat(contacto): agregar datos de contacto

\* | ab943e9 feat: merge features info y contacto

|\\|

| \* b41241f (feature/info) feat(info): agregar sección información

\* | 75f2cc2 feat(contacto): agregar datos de contacto

|/

\* f721d0f (origin/feature/reportes, origin/develop, feature/reportes) feat(ui): implementar navegación mobile

\* cf83b5e feat(ui): agregar nuevos componentes de interfaz

\* 0dabf50 chore(release):preparar version 1.0

| \*   5f0126d (refs/stash) WIP on master: ed15266 chore(release):preparar version 1.0

| |\\

| | \* 85ce36c index on master: ed15266 chore(release):preparar version 1.0

| |/

| \* ed15266 (HEAD -> master, origin/master, origin/HEAD, release/v1.0) chore(release):preparar version 1.0

|/

\* a04d218 (feature/login) feat(login):agregar funcionalidad login

\* 3bbc5ec feat: versión inicial





\## Flujo Seguido



\### \*\*Ramas Principales\*\*

\- `main`: Rama de producción

\- `develop`: Rama de integración



\### \*\*Ramas de Soporte\*\*

\- `feature/\*`: Nuevas funcionalidades

\- `release/\*`: Preparación de releases



\### \*\*Comandos Ejecutados\*\*

```bash

\# 1. Crear features

git checkout -b feature/info

git checkout -b feature/contacto



\# 2. Merge a develop

git merge feature/info

git merge feature/contacto



\# 3. Crear release

git checkout -b release/v1.0



\# 4. Merge a main

git checkout main

git merge release/v1.0

