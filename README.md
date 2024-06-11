# 0.21

This repository is dedicated only for Woodworking workbench version [0.21 stable](https://github.com/dprojects/Woodworking/releases/tag/0.21).

# How to create translation

1. Download exact `.ts` file.
2. Make translations of the `.ts` file. You can use any editor for that.

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

	**Note:** Do not change the string between `<source>` and `</source>`, only the translation.

3. Create pull request with your new `.ts` file.

	**Note:** Please do not add `.qm` file, because the `.ts` file need to be verified and after accepting pull request I will recreate the `.qm` file.
