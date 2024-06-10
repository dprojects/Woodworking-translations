# Rules for translation community

* Please create pull request with *.ts and *.qm files. You have to add *.ts file as well for further translation development and updates.
* To add translation select exact branch. For example if you want add translation for Woodworking workbench 0.21 version you have to open pull request at 0.21 branch.
* You should add translations only for [stable releases](https://github.com/dprojects/Woodworking/releases) because the code will not change.

# How to create translation

You can create your own `Woodworking` workbench translation with the following steps:

* Generate `.ts` file. At `Xubuntu 22.04 LTS` in `Woodworking` directory:
	
	```
	pylupdate5 `find . -name "*.py"` -ts translations/pyfiles.ts
	```
	
* Rename `pyfiles.ts` e.g.:

	```
	mv ./translations/pyfiles.ts ./translations/Woodworking_pl.ts
	```
	
	**Note:** Replace `pl` with your language code.
	
* Make translations of the `.ts` file. You can also use editor for that.

	* For example this entry below:
	```
	<source>Step 2. Custom CSS rules for each cell (edit or add):</source>
	<translation type="unfinished"></translation>
	```
	* should be replaced with:
	```
	<source>Step 2. Custom CSS rules for each cell (edit or add):</source>
	<translation>Krok 2. Własne ustawienia CSS dla komórki:</translation>
	```

* Generate `.qm` files:
	
	```
	sudo apt-get install qttools5-dev-tools
	/usr/lib/x86_64-linux-gnu/qt5/bin/lrelease ./translations/Woodworking_pl.ts
	```

* Set your language at FreeCAD preferences.
