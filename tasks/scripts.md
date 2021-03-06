# scripts

## Implementation status

### Gulp: Implemented
### Grunt: None

## Options

  * src
    * entry point
    * default: ``"<%= paths.app %>/scripts/main.js"``
  * filename
    * destination filename
    * default: ``"main.js"``
  * moduleSystem
    * default: ``"browserify"``
    * possible: ``"browserify"``, ``null`` (future: ``"requirejs"``)
  * transpiler
    * default: ``null``
    * possible: ``null``, ``"babel"``
  * bower
    * include bower components (if browserify is used)
    * default: ``false``
  * templates
    * default: ``"handlebars"``
  * dest
    * destination path
    * default: ``"<%= paths.tmp %>/scripts"``
  * debug
    * should the sourcemaps be generated
    * default: ``false``
  * moduleSystemConfig
    * aliases
      * used with ``browserify``
      * options passed to aliasify module
      * default: ``{}``
    * nodePath
      * used with: ``browserify``
      * used node paths
      * default: ``process.env.NODE_PATH.split(":").concat("/<%= paths.app %>/scripts")``
  * transpilerOptions
    * options passed to transpiler module (if used)
    * default: ``{}``
  * templateOptions (not used with browserify)
    * src
      * path where the template file will be saved
      * default: ``"<%= paths.app %>/scripts/templates/**/*.hbs"``,
    * namespace
      * the valiable name used for templates
      * default: ``"JST"``
