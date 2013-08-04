# Description

This is just a skeleton application, with ExtJS as frontend and using Gradle to create artifact for easy deployment and version controll.
---
  - ExtJS 4.2.1.833
  - Gradle 1.6

# Prerequisites
---
  - [Sencha CMD](http://www.sencha.com/products/sencha-cmd/download)
  - [Gradle](http://www.gradle.org)


# Instructions

To simply build the application

	gradle war

This will minify the app using sencha cmd, and generate a war with default settings (Version etc)

More advanced features

	gradle war -Dversion=0.2 -DbuildNumber=0001

This will build the application, and set the version according to input. Usefull for instance when doing continuous integration with a build tool like TeamCity, to automagically version your app. 

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
