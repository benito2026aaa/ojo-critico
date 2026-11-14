# Subir Ojo Crítico a GitHub

Repositorio destino: https://github.com/benito2026aaa/ojo-critico
Rama: `main`

La integración GitHub de ChatGPT devolvió un error 403 al intentar escribir. Este ZIP contiene los archivos listos para subirlos desde tu equipo.

## Opción A: Git desde VS Code (recomendado)

Descomprime el ZIP y abre la carpeta `ojo-critico-benito2026aaa` en VS Code. Abre **Terminal > Nueva terminal** y ejecuta:

```bash
git init -b main
git add .
git commit -m "feat: primera versión interactiva Ojo Crítico"
git remote add origin https://github.com/benito2026aaa/ojo-critico.git
git push -u origin main
```

Si el repositorio ya contiene commits en `main`, no fuerces `git push`: revisa primero los cambios del remoto.

## Opción B: subir desde GitHub

Abre https://github.com/benito2026aaa/ojo-critico, elige **Add file > Upload files**. Extrae el ZIP y arrastra **los archivos de dentro de la carpeta**, no el ZIP, manteniendo la estructura de subcarpetas. Confirma el commit a `main`.

Archivos principales: `index.html` (web), `motion/index.html` (composición), `README.md` (instrucciones), `.gitignore`.

Nota editorial: el sitio es una maqueta; revisa las cifras del SíseVe y los contenidos antes de publicarlo.
