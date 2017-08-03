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

4. Instale Atom IDE

   1. Instalando plugin de Typscript en Atom: atom-typescript

![](/assets/screenshot_typescript_plugin_install_on_atom.png)

* Instalando el plugin de atom-beautify

![](/assets/screenshots_atom_install_plugin_atom-beautify.png)

**Generando proyecto básico en Angular**

* Creando proyecto

`sudo  ng new test1`

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



