# Adobe Experience Manager 6 Extension: Customizing the foundation page dialog

This is a sample package showing how to extend the foundation page dialog in order to customize the different views of the page properties:
* Add custom field to “Edit Page Properties” and “Bulk Edit Page Properties” views
* Hide Advanced tab in “Create Page” view
* Show Thumbnail tab only in “Create Page” view (hide it in "Edit Page Properties" view)
* Make an existing field required and add custom validation to another field

## Building 
 
This project uses Maven for building. Common commands:

From the project directory, run ``mvn clean install content-package:install`` to build the bundle and content package and install to a CQ instance.

## Using with VLT 
 
To use vlt with this project, first build and install the package to your local CQ instance as described above. Then cd to `src/main/content/jcr_root` and run

    vlt --credentials admin:admin co http://localhost:4502/crx/-/jcr:root . --force

Once the working copy is created, you can use the normal ``vlt up`` and ``vlt ci`` commands.