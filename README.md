# Update:

The tool has been superseeded by a fully fledged appearance editor and as such, this one is obsolete. The repository will remain available for anyone that wants to build their own tool on it. Thanks to everyone who used the tool.

# cp77_hairdresser

![image](https://i.imgur.com/UapYJbV.png)

A cross-platform program for changing hairstyle in Cyberpunk 2077.
Implements UI and script style editor.

Inspired by: https://www.nexusmods.com/cyberpunk2077/mods/291

# Installation (for users)

* Install Python3 (64 bit, enable "Add to PATH" checkbox during install)

```
pip install pyqt5
pip install cp77_hairdresser
```

# Running the program

To run GUI, execute
```
python -m cp77_hairdresser.editor_gui
```

There is also script version of the program. To run it, execute
```
python -m cp77_hairdresser.editor
```

Use `-h` flag to display help information on how to use the script version.

# Creating a package for PIP (my own reminder)

First, edit the version in `setup.py`.

```
python3 setup.py sdist bdist_wheel
python3 -m twine upload --repository testpypi dist/* #for test pypi
python3 -m twine upload --repository pypi dist/* #for pypi
```
