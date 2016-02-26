# AEM Granite Dynamic Select

This project adds the ability to use a dynamic datasource within AEM Granite (Touch) dialogs.

![Dynamic Select](https://raw.githubusercontent.com/auniverseaway/aem-touch-dialog-select/master/assets/thumbnail.png)

##There are two components to achieve this.

1. datasource component - This component / rescoureType is designed to be very generic in nature. This is all the logic you need.
2. dyanmic-dialog - This component creates the static list of items as well as referencing itself to generate a dynamic list.

##Usage

### Option 1 - Package
There is a CRX package that can be deployed directly. It will populate apps/aem-touch-dynamic-select/components. You can then test the demo component (dynamic-dialog).

### Option 2 - Pull into your project
You can pull both components into your project. You really only need the datasource. Use dynamic-dialog as a reference.

Dynamic-dialog is meant as a demo for your needs. The datasource component requires three parameters to work correctly:

1. value - this is the value that should be stored as a JCR property.
2. name - this is the value used for the name to display in the select field.
3. path - this is the endpoint where the list of items is located.

##Notes

* The dynamic-dialog component is in the "General" component group.
* Within this repository is a content package that can be used as a drop-in utility for any AEM site. 
* It's *recommended* that you pull these components into your project.