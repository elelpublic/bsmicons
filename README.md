bsmicons
========

Missing icons in the style of [Bootstrap](http://getbootstrap.com/components/) 
and [Font Awesome](http://fortawesome.github.io/Font-Awesome/). 
Complete with build system based on [Font Custom](http://fontcustom.com/).

This project provides vector images (SVG) and a build system to create css ready icons sets from it.

Mainly we provide icons which we feel missing in Bootstrap and Font Awesome.

To use this project to build icon sets, you need to have font custom installed on you system.

Installation of Font Custom
---------------------------

When you have Ubuntu it's in your package manager. 

When you're on a Mac with brew, see here: http://fontcustom.com/#installation

When you're on a Mac with Macports:

	sudo port install fontforge
	sudo port install rb-rubygems
	sudo gem install fontcustom

Use Fontcustom with Docker
--------------------------

In case you cannot install fontcustom for some reason, you can use the Docker image thomaswelton/fontcustom:

	docker run -ti -v <YOUR_LOCAL_WORKSPACE_DIR>:/workspace thomaswelton/fontcustom /bin/bash
	cd /workspace/bsmicons
	fontcustom compile src/svg/ -o build/

See: https://registry.hub.docker.com/u/thomaswelton/fontcustom/

Works with boot2docker 1.3 and up.




