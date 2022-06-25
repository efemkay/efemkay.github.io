---
title: "Installing Windows Font on Linux"
categories:
  - Homelab
  - Linux
permalink: "/notes/petroleum-economics/windows-font-on-linux/"
---

- ### Core Windows Font
	- this will install MS Windows core fonts i.e. Arial etc.
	- Optional
		```shell
		sudo add-apt-repository multiverse
		sudo apt update
		```
	- Optional if installing
		```shell
		# install FontForge will help doing the font conversion
		# install MS Cabinet file unpacker. required if u didn't install corefonts first
		sudo apt-get install fontforge
		sudo apt-get install cabextract
		```
	- sudo apt-get install fontforge
	- Install the Microsoft Cabinet file unpacker. This is required for the next script to successfully install the fonts.
	- sudo apt-get install cabextract
	- Install the font from repository
	  `sudo apt install ttf-mscorefonts-installer`
	- Update the font cache
	  `sudo fc-cache -f -v`
- ### Vista Fonts
	- The following steps is in addition to the above, to install Vista related fonts i.e. Calibri
		```shell
		  wget https://gist.github.com/maxwelleite/10774746/raw/ttf-vista-fonts-installer.sh -q -O - | sudo bash
		```

## References
- https://itsfoss.com/install-microsoft-fonts-ubuntu/
- https://itectec.com/ubuntu/ubuntu-how-to-get-calibri-font-to-display-nicely-duplicate/
	- to make Windows font looks like by disabling antialiasing
