Download GDAL http://www.gisinternals.com/release.php
Step for installing http://www.gisinternals.com/release.php


## Installation

* Install Python and GDAL for Python
  * Download and install Python: 
    * go to [https://www.python.org/downloads/](https://www.python.org/downloads/) and download the latest version for Windows, download the latest 2.7.2 version of Python (rather than the 3.x Python version)
	* click on the download file to start the installation, install Python with default options and directions
	* after installation, from Windows Start menu, go to Python IDLE (Python GUI) to find out waht version of Python (32 bit or 64 bit)
		![Python IDLE](/img/01_PythonShell.png)
	Make a note of MSC number (MSC v.1500) and 32 bit or 64 bit for GDAL installation.
	
  * Download and install GDAL core and GDAL for Python: 
    * go to [Tamas Szekeres’ Windows binaries](http://www.gisinternals.com/release.php) and download the appropriate GDAL Binary
	* select the release that match your MSC number and your Python system (32 bit or 64 bit) by verifying IDLE above
		![Select GDAL release](/img/02_GDALDownload.png)
	* select .msi file to download from the list of binaries to download
		![Download GDAL binaries](/img/03_GDAL_msi.png)
	  * download GDAL core (gdal-111-1500-core.msi) with Generic installer for the GDAL core components, then install this GDAL core with default setting
	  * download GDAL for Python (GDAL-1.11.3.win32-py2.7.msi) that matches with the Python version above, then install this GDAL for Python

  * Add GDAL to path variables
    * Right click on "Computer" on the desktop and go to "Properties"
	* Select "Advanced system settings"
		![Advanced system settings](/img/04_Variables.png)
	* Click on "Environment Variables"
		![Advanced system settings](/img/04_Variables.png)
	* Add 2 new variables
		Name             | Value
		---------------- | -------------
		GDAL_DATA        | C:\Program Files (x86)\GDAL\gdal-data
		GDAL_DRIVER_PATH | C:\Program Files (x86)\GDAL\gdalplugins
	
		![Advanced system settings](/img/05_Add _Variables.png)
	* Add GDAL core path (;C:\Program Files (x86)\GDAL) to the end of variables "Path"
	
	Note: if you install Python 64 bit, the value should be C:\Program Files\GDAL
	
* Install Eclipse and PyDev on Windows 
  
  * Download and install Eclipse: 
    * go to [https://eclipse.org/downloads](https://eclipse.org/downloads) for downloading Eclipse Installer, choose Windows 64 bit if you are using 64 bit version of Windows, otherwise choose Windows 32 bit
		![Download Eclipse Installer](/img/1_DownloadEclipse.png)
	* from the screen presented to Eclipse Download - Select a mirror, then click on "Download" button to download executable file 
		![Select mirror](/img/2_DownloadEclipse.png) 
	* click on the download file (should be eclipse-inst-win64.exe) to start Eclipse installer
		![Start Eclipse Installer](/img/3_InstallEclipse.png) 
	* choose Eclipse IDE package to install, "Eclipse IDE for Java developers" is recommended
	* choose the installation folder, and click on "Install" button to begin the instalation
		![Choose Installation Folder](/img/4_InstallationFolder.png) 
		
	Note: you can also download an Eclipse Packavge from [https://eclipse.org/downloads](https://eclipse.org/downloads), then extract the .zip file and move to a desired folder (as your Eclipse installation folder) and run eclipse.exe from there
	
  * Launch Eclipse
	* Execute eclipse.exe within the eclipse folder, the popup for selecting a workspace for storing the projects
		![Launch Eclipse](/img/5_LaunchEclipse.png)
  
  * Install PyDev with the update site
	* From Eclipse IDE, select menu Help > Install New Software
		![Install pyDev](/img/6_Install_PyDev.png)
    * Click on button "Add" for selecting a site and enter "PyDev and PyDev Extensions" in Name and "http://pydev.org/updates" in Location
		![Install PyDev](/img/7_Install_PyDev_update_sites.png)
	* Select "Select All" button and click "Next" button to start the installation
		![Install PyDev](/img/8_Select_PyDev_Items.png)
	* then accept the terms of license agreement and click on "Finish" button
	
