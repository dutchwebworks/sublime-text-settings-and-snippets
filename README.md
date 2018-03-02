# Sublime Text settings and snippets

*By Dennis Burger, march 2018*

Here are my **Sublime Text 3 settings** and **snippets** that I'm using.

## Package control

You install them by first installing [Package Control](https://packagecontrol.io/installation). Then inside Sublime Text you open the **command-pallet** hitting `shift + cmd + p` on macOS or `ctrl + shift + p` on Windows and type `pack install`. Then search for and install the below list of packages one by one.

## Sublime Text Packages

* AdvancedNewFile
* Emmet
* FileDiffs
* Git
* GitGutter
* Material Theme
* Open-Include
* Package Control
* Pug
* SCSS
* SideBarEnhancements
* SublimeCodeIntel
* Vue Syntax Highlight
* Vuejs Complete Package

## Keyboard shortcuts

Inside the macOS and Windows Sublime Text respected `Default (OSX).sublime-keymap` and `Default (Windows).sublime-keymap` are some **handy keyboard shortcuts** that I use a lot. 

## Snippets

Inside the `snippets/` directory are my list of Sublime Text snippets. You can copy these **to your own Sublime Text directory**:

### macOS

```bash
~/Library/Application Support/Sublime Text 3/Packages/User/snippets
```

### Windows

```bash
%APPDATA%\Sublime Text 3/Packages/User/snippets
```

## FileDiffs paths to Beyond-Compare

The FileDiff package allows you to open two files from Sublime Text to a file diffing tool like Beyond-Compare. The path to the Beyond-Compare diff. tool is ofcourse different per operating-system. Here are my macOS and Windows settings for this Sublime Text 3 package.

Below are the settings file for FileDiffs.

### macOS

For macOS make sure you've installed the Beyond-Compare **commandline** tools from inside the Beyond-Compare application. So the below `/usr/local/bin/bcompare` is available.

```json
{
     // "cmd": ["/usr/local/bin/bcomp", "$file1", "$file2"]
     "cmd": ["/usr/local/bin/bcompare", "$file1", "$file2"]
     // "trim_trailing_white_space_before_diff": false
     // "expand_full_file_name_in_tab": false
     // "apply_tempfile_changes_after_diff_tool": false
}
```

### Windows

```json
{
	 // "cmd": ["/usr/local/bin/bcomp", "$file1", "$file2"]
	 "cmd": ["C:\\Program Files\\Beyond Compare 4\\BCompare.exe", "$file1", "$file2"]
	 // "trim_trailing_white_space_before_diff": false
	 // "expand_full_file_name_in_tab": false
	 // "apply_tempfile_changes_after_diff_tool": false
}
```