# Steam-CSS-Skins
CSS tweaks to alter browser-based steam client features.

# Examples
All skins have before and after screenshots in their folders.

# Basic usage
First, find your `libraryroot.css` file. Make a backup of the original file in case you want to roll back your changes.

Next, Choose a skin. Download the corresponding `libraryroot.css` file. Replace the file with the same name in your `steamui/css` folder.

On a default windows installation, the full path to the file is `C:\Program Files (X86)\Steam\steamui\css\libraryroot.css`.

Changes are immediate. No restart of steam is necessary.

# Manually inserting rules
If you don't want to replace the original file, you may simply copy/paste the contents of a skin's `skin.css` file to the end of your `libraryroot.css` file.

CSS files are simply text files. If you're on windows, you can edit them with notepad.

# Modifying skins
All skins are commented to identify what each CSS rule is meant to do. If you have any CSS knowledge, you should be able to modify those rules to suit your preference.

# Combining skins
If you want to combine different skins, copy the contents of all corresponding `skin.css` files to the end of your existing `libraryroot.css` file. Some skins may have conflicting rules. If you can't

# Preventing Steam from undoing changes
Every time you start Steam, it checks the integrity of every file and re-downloads files that have been changed.

To prevent this, add the `-noverifyfiles` and `-norepairfiles` flags to your steam shortcut by right-clicking it, clicking "Properties", and adding them to the `Target` field.

Here's an image of what it should look like:
![Image of shortcut properties](https://i.imgur.com/kVdvuOJ.jpg)

# Is this safe?
You can examine every file for yourself. CSS is capable of doing two things: Change the visual properties of elements in a web page, and load external assets such as images into the web page. None of the skins in this repository load external assets.

No additional requests will be made to any server as the result of using these CSS rules. Note that the original CSS does load some external assets, and those are kept unchanged.

# I want something different
Post an issue describing what you want and I'll see what I can do.
