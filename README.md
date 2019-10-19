Page Icon
=========

## Description
+ The module allows to assign page related icons (font awesome) shown in the backend.  
	If a template or process related icon is set it will be overwritten.
+ During install the module creates a field **page_icon** where the data is stored and assign it to all templates.
+ An *InputfieldIcon* will be shown under the Settings tab in the page edit area and can only be accessed from here. The field does not appear on the Content tab.

---

## Good to know
+ The icon is shown in the page tree via a hook in `Page::getIcon()`
+ The page property **page_icon** is known by *ProcessList* (since PW 3.0.143) and *AdminThemeFramework*
+ To provide the option to add an icon to pages using a template with the **noGlobal** flag (e.g. admin, language), the corresponding field must be added manually.