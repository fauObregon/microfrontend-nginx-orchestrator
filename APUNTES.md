# Ejercicio de Micro-Frontend con Nginx

## Espacio de trabajo

Creeremos un directorio llamado `microfrontend-nginx-orquestator/` con el siguiente comando:

```powershell
mkdir microfrontend-nginx-orchestator 
```

No movemos al directorio creado

```powershell
cd microfrontend-nginx-orchestator
```

### Creamos los proyectos

Utilizaremos 3 proyectos de tres tecnologias  distintas, **Angular**, **Vue** y **React**

#### Crear mf-angular

Ejecutamos el siguiente comando

```powershell
ng new mf-angular
```

Resultado

```powershell
? Which stylesheet format would you like to use? CSS             [ https://developer.mozilla.org/docs/Web/CSS                     ]
? Do you want to enable Server-Side Rendering (SSR) and Static Site Generation (SSG/Prerendering)? No
CREATE mf-angular/angular.json (2707 bytes)
CREATE mf-angular/package.json (1079 bytes)
CREATE mf-angular/README.md (1090 bytes)
CREATE mf-angular/tsconfig.json (889 bytes)
CREATE mf-angular/.editorconfig (290 bytes)
CREATE mf-angular/.gitignore (590 bytes)
CREATE mf-angular/tsconfig.app.json (277 bytes)
CREATE mf-angular/tsconfig.spec.json (287 bytes)
CREATE mf-angular/.vscode/extensions.json (134 bytes)
CREATE mf-angular/.vscode/launch.json (490 bytes)
CREATE mf-angular/.vscode/tasks.json (980 bytes)
CREATE mf-angular/src/main.ts (256 bytes)
CREATE mf-angular/src/favicon.ico (15086 bytes)
CREATE mf-angular/src/index.html (308 bytes)
CREATE mf-angular/src/styles.css (81 bytes)
CREATE mf-angular/src/app/app.component.html (20239 bytes)
CREATE mf-angular/src/app/app.component.spec.ts (957 bytes)
CREATE mf-angular/src/app/app.component.ts (319 bytes)
CREATE mf-angular/src/app/app.component.css (0 bytes)
CREATE mf-angular/src/app/app.config.ts (235 bytes)
CREATE mf-angular/src/app/app.routes.ts (80 bytes)
CREATE mf-angular/src/assets/.gitkeep (0 bytes)
✔ Packages installed successfully.
    Successfully initialized git.
```

#### Crea proyecto mf-vue

Ejecutamos el siguiente comando

```powershell
vue create mf-vue
```

Resultado

```powershell


Vue CLI v5.0.8
? Please pick a preset: Default ([Vue 3] babel, eslint)


Vue CLI v5.0.8
✨  Creating project in D:\LABS\microfrontend\microfrontend-nginx-orchestator\mf-vue.
🗃  Initializing git repository...
⚙️  Installing CLI plugins. This might take a while...


added 878 packages, and audited 879 packages in 55s

100 packages are looking for funding
  run `npm fund` for details

4 moderate severity vulnerabilities

To address issues that do not require attention, run:
  npm audit fix

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
🚀  Invoking generators...
📦  Installing additional dependencies...


added 95 packages, and audited 974 packages in 12s

112 packages are looking for funding
  run `npm fund` for details

4 moderate severity vulnerabilities

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
⚓  Running completion hooks...

📄  Generating README.md...

🎉  Successfully created project mf-vue.
👉  Get started with the following commands:

 $ cd mf-vue
 $ npm run serve


```

#### Crear proyecto mf-react

Ejecutamos el siguiente comando.

```powershell
npx create-react-app mf-react
```

Resultado

```powershell
Creating a new React app in D:\LABS\microfrontend\microfrontend-nginx-orchestator\mf-react.

Installing packages. This might take a couple of minutes.
Installing react, react-dom, and react-scripts with cra-template...


added 1493 packages in 2m

258 packages are looking for funding
  run `npm fund` for details

Initialized a git repository.

Installing template dependencies using npm...

added 68 packages, and changed 1 package in 16s

262 packages are looking for funding
  run `npm fund` for details
Removing template package using npm...


removed 1 package, and audited 1561 packages in 5s

262 packages are looking for funding
  run `npm fund` for details

8 vulnerabilities (2 moderate, 6 high)

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.

Created git commit.

Success! Created mf-react at D:\LABS\microfrontend\microfrontend-nginx-orquestator\mf-react
Inside that directory, you can run several commands:

  npm start
    Starts the development server.

  npm run build
    Bundles the app into static files for production.

  npm test
    Starts the test runner.

  npm run eject
    Removes this tool and copies build dependencies, configuration files
    and scripts into the app directory. If you do this, you can’t go back!

We suggest that you begin by typing:

  cd mf-react
  npm start

Happy hacking!
```

