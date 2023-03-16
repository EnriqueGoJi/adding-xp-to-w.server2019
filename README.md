# adding-xp-to-w.server2019
Let's add a Windows XP SP3 Spanish to a Windows Server with Domain Controler Role.

If your XP is into another SP (1 or 2) you need to install the SP3 package.

After installing both systems, and promoting the server to dc and creating the domain with the lower compatibility mode (Windows 2008 Server) we need to config the XP.

****XP Configuration****

We are going to change the languaje in the regional settings.

We need to modify some files in this rute of the registry.
**HKEY_LOCAL_MACHINE/SYSTEM/ControlSet001/Control/NIs/Language.**

Set the default and install_Languaje key with the code you want. (I use the United Kingdom, 0809)

The keys are in the languaje_key file.

Then you need to config in the regional configurations all the options with the English languaje.

After all this you can restart the machine and isntall the update.

Tutorial Wikihow: https://es.wikihow.com/cambiar-el-idioma-de-tu-computadora-en-Windows-XP

***Update****

Import the archive (WindowsXP-KB969442-x86-ENU) and run it.

After the installation restart again.

****Domain Join****

Try to add it. You must need the admin user and pass.

If there is anny error, check out the previus steps. Especially the languaje one.

