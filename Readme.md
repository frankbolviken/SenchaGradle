# Description

This is just a skeleton with the latest ExtJS version (ExtJS 4.2.1), and Gradle.

# Prerequisites
---
  - [Sencha CMD](http://www.sencha.com/products/sencha-cmd/download)
  - [Gradle](http://www.gradle.org)


# Instructions

To simply build the application

	gradle war

This will minify the app using sencha cmd, and generate a war with default settings (Version etc)

# Coming up
Jasmine support
Deployment to servers (Test, Stage, Prod etc)



# SenchaGradle/app

This folder contains the javascript files for the application.

# SenchaGradle/resources

This folder contains static resources (typically an `"images"` folder as well).

# SenchaGradle/overrides

This folder contains override classes. All overrides in this folder will be 
automatically included in application builds if the target class of the override
is loaded.

# SenchaGradle/sass/etc

This folder contains misc. support code for sass builds (global functions, 
mixins, etc.)

# SenchaGradle/sass/src

This folder contains sass files defining css rules corresponding to classes
included in the application's javascript code build.  By default, files in this 
folder are mapped to the application's root namespace, 'SenchaGradle'. The
namespace to which files in this directory are matched is controlled by the
app.sass.namespace property in SenchaGradle/.sencha/app/sencha.cfg. 

# SenchaGradle/sass/var

This folder contains sass files defining sass variables corresponding to classes
included in the application's javascript code build.  By default, files in this 
folder are mapped to the application's root namespace, 'SenchaGradle'. The
namespace to which files in this directory are matched is controlled by the
app.sass.namespace property in SenchaGradle/.sencha/app/sencha.cfg. 
