# Bungie Clan List for Joomla!

Display your Destiny 2 Clan's Roster in Joomla!.

# Setting Up Development Environment on Windows

1. Install XAMPP
   - (Optional) Setup a virtual host for your Joomla! install
1. Install Joomla!
1. Clone repository to desired location
1. Create a zip of all files within the repository
1. Install the extension in Joomla! via the zip you just created
1. Open the Joomla! installation directory within the XAMPP files
1. Delete the following folders:
   - `<joomla_install_root>\components\com_bungieclanlist`
   - `<joomla_install_root>\administrator\components\com_bungieclanlist`
1. Run the following in Command Prompt:
   ```
   mklink /J "<joomla_install_root>\components\com_bungieclanlist" "<source_root>\site"
   mklink /J "<joomla_install_root>\administrator\components\com_bungieclanlist" "<source_root>\admin"
   mklink /H "<joomla_install_root>\administrator\components\com_bungieclanlist\bungieclanlist.xml" "<source_root>\bungieclanlist.xml"
   ```
