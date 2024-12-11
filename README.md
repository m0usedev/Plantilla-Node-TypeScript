# Pasos para configurar el proyecto

1. Clona este repositorio

```cmd
git clone https://github.com/m0usedev/Plantilla-Node-TypeScript.git .
```

3. Elimina la relación con el repositorio remoto

```cmd
git remote remove origin
```

3. Instala las dependencias

```cmd
npm install --save-exact
```

4. Actualizar dependencias
   - `npm run ncu`: comprueba si hay alguna dependencia con nuevas versiones.
   - `npm run ncu -- -u -f "dependencia1 dependencia1 ..."`: comando para actualizar a la ultima version una dependencia especifica.
   - `npm run ncu -- -u`: para actualizar todas las dependencias.
5. Scripts disponibles:
   - `dev`: para ejecutar el modo desarroll con ts-node-dev en ./src/main.ts.
   - `tsc-alias`: Para hacer uso de `tsc-alias`. Que sirve para reemplazar las rutas de alias con rutas relativas después de la compilación.
   - `build`: "tsc && tsc-alias"
   - `re-build`: que sirve para recompilar ts cuando ya lo hiciste anteriormente, eliminando la carpeta dir previamente.
   - `tsc`: para tener acceso a tsc.
   - `build`: elimina la anterior compilacion de .dist/ y vuelve a compilar el codgio ts.
   - `lint:base`: para tener acceso a `eslint`.
   - `lint:check`: para detectar fallos en el codigo ts en src.
   - `lint:fix`: para arreglar todos los fallos posibles en los archivos ts de src.
   - `ncu`: para tener acceso a `ncu`.
