#installing smartypdt.

# Installation #

This page describes the installation steps for smartypdt (**Thanks to matei.dragu for his comments!**)

# Requirements #
Download PDT 3.x / Studio 10.x all-in-one from Zend's site

# Install #
You requested info about how to install SmartyPDT 0.9.1 on Juno, so i will try to explain the steps:

  * Be sure that the .TPL files are not associated with any content type (file type). In Eclipse, go to Window->Preferences->General->Content Types and under the Text section check HTML and PHP Content Type If you see that the .TPL is associated with anything, just delete those entries.
  1. Go to Help-> Install New Software
    * At the Work With section click on the Add... button. Give the new "Site" a name and set the location with http://smartypdt.googlecode.com/svn/trunk/org.eclipse.php.smarty.updatesite/  ,then click OK. Go back to the Install New Software window and select the newly added "site". If the "Group items by category" check-box is checked, uncheck it. Now you should be able to see 1 item in the software list named "Smarty Feature"
  1. Select the Smarty Feature, click Next> and from here afterwards it shouldn't be a problem.
    * If you are prompted that this is an unsigned package, just ignore the warning and install it anyway.
  1. After the installation completes, restart Eclipse and it should be working.
  1. Define a default PHP executable of type 'Zend Debugger' (only if you install vanilla Eclipse PDT):
    * In Eclipse go to Window->Preferences->PHP->PHP Executables Click on the Add button. Enter a name for that executable definition, for example "PHP localhost", complete the 2 fields which ask you for the PHP executable path (the PHP binary CLI executable) and php.ini path. Be sure that the PHP debugger is the Zend Debugger.