CONTENTS OF THIS FILE
---------------------

 * Introduction
 * Recommended modules
 * Installation
 * Configuration
 * More information

INTRODUCTION
------------

This Drupal 7 module is designed to fix Entity Reference (ER) fields saving on
multilingual content types (Content Translation + i18n).

 * When a multilingual node is created or saved, this module will save the
   references to entities in the same language of parent node. Doesn't
   matter if you have selected options in other languages. This module will
   handle things for you.

 * It is highly recommended to make this module work in conjunction with
   "Translated Entity Reference" module. Make sure to select the option
   "Select only nodes matching the parent's language" for all ER fields
   once this other module is enabled.

 * This module works only with ER fields that point to nodes and taxonomies.

RECOMMENDED MODULES
-------------------

 * Translated Entity Reference (https://www.drupal.org/project/translated_entityreference):
   It filters "Entity Reference" fields options given parent's or interface
   language.

   However, if you choose parent's language for your fields there is a problem:
   when you change the language of a node while creating or editing them it
   doesn't automatically change the ER field options to match parent's
   language. And this is the reason why I programmed "Translated Entity
   Reference Save" module.

INSTALLATION
------------

 * Install as you would normally install a contributed Drupal module. See:
   https://drupal.org/documentation/install/modules-themes/modules-7
   for further information.

CONFIGURATION
-------------

 * Just enable the module. There is no specific configuration for this module.

MORE INFORMATION
----------------

 * https://www.drupal.org/node/2762971
