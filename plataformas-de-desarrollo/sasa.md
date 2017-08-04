1. Instalación de gestor de paquetes NPM
   1. Instalación de npm
      * `npm install -g npm`
2. Instalación de NodeJS
   1. Instalación via npm
      * `sudo npm install nodejs`
3. Instalación de Angular 2/4

   1. Instalación de Angular CLI \(Comand Line Interface basado en el Ember.js\)

      * `npm install -g @angular/cli`
      * Parametro "-g": instalación glocal
      * @angular/cli

4. Instalando Atom IDE y Plygin

   * Instalando los plugins de Atom : atom-typescript, linter, editorconfig, fileicons \([https://denisvuyka.github.io/2016/05/29/angular2-atom-quickstart.html\](https://denisvuyka.github.io/2016/05/29/angular2-atom-quickstart.html%29\)
   * Typscript en Atom: atom-typescript

![](/assets/screenshot_typescript_plugin_install_on_atom.png)

* Instalando el plugin de atom-beautify

![](/assets/screenshots_atom_install_plugin_atom-beautify.png)

**Nota: **Posiblementa al modificar tu codigo fuente vas a requerir instalar dependencias de atom-typescript

![](/assets/atom_plugin_linter_install_dep.png)

**Generando proyecto básico en Angular**

* Creando proyecto

`sudo  ng new bitfy`

**nota:** no se puede crear proyectos con nombre "test", que empiece con numeros.

![](/assets/screeshots_projects_name_invalids.png)

* Carpetas de proyecto:

![](/assets/screenshots_folder_project_test1.png)

**nota:** dado caso que quieras establecer Yarn como package manager: `ng set --global packageManager=yarn`

* Ejecutando servidor web

`ng server`

**Compilando proyecto **

* Compilación para producción

`sudo ng build --prod`

** Generando unidades de pruebas**

`sudo ng serve --prod`

* Genera la carpeta dist

**Publicando para producción**

`sudo ng serve --prod`

* Genera la carpeta dist

![](/assets/screehshot_folder_after_build_prod.png)

** Creando carpetas de proyecto**

`cd src/app`

* Carpeta src/app/private: contenido para usuarios autenticados
  * `mkdir private`
* Carpeta src/app/common: contenido para compartir a toda la aplicación
  * `mkdir common`
* Carpeta src/app/public: contenido para todo el publico
  * `mkdir public`
    ![](/assets/screen_project_folders_app.png)

Creando componente de Autenticación

* Creando componente project-list

  * `ng generate component project-list`

  Resultado:

  * `installing component`
    `create src/app/private/project-list/project-list.component.css`
    `create src/app/private/project-list/project-list.component.html`
    `create src/app/private/project-list/project-list.component.spec.ts`
    `create src/app/private/project-list/project-list.component.ts`
    `update src/app/app.module.ts`

  ![](/assets/screenshot_project-list.png)

* Creando componente header

  * `mkdir src/app/common/layout/header`
  * `cd src/app/common/layout/header` 
  * `ng generate component header`

  Resultado:

  * installing component

    `create src/app/common/layout/header/header.component.css`

    `create src/app/common/layout/header/header.component.htmlloader!./src/styleshe`

    `create src/app/common/layout/header/header.component.spec.ts`

    `create src/app/common/layout/header/header.component.ts`

    `update src/app/app.module.ts`

  ![](/assets/screenshot_project_folder_header.png)



