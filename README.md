# adding-xp-to-w.server2019
Let's add a Windows XP SP3 Spanish to a Windows Server with Domain Controler Role.

If your XP is into another SP (1 or 2) you need to install the SP3 package.

After installing both systems, and promoting the server to dc and creating the domain with the lower compatibility mode (Windows 2008 Server) we need to config the XP.

****XP Configuration****

We are going to change the languaje in the regional settings.

We need to modify some files in this rute of the registry.
HKEY_LOCAL_MACHINE/SYSTEM/ControlSet001/Control/NIs/Language.

