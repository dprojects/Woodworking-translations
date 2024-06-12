# 0.22 (not available yet)

This repository is dedicated only for Woodworking workbench version 0.22 stable.

**Note:** Currently this version is not available so it is used only for [development](https://github.com/dprojects/Woodworking) master branch testing purposes. For testing purposes you can change `version` inside `package.xml` file from `0.21.2.33771` to `0.22.2.33771` and choose drop down menu `Woodworking -> Download and update all translations`. Please do not add translations here because the code will change and your translations will not be valid.

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
