# Sublime Gem Browser 0.3-alpha

For Ruby projects using the Bundler gem.

This plugin allows you to quickly access the code of a gem that you have installed via Bundler in the current project. When you select a gem, a new Sublime Text 2 window will open with the code ready for inspection.

Tested on OSX with RVM, Xubuntu with rbenv and Windows with RubyInstaller
# How to Use
* In ST2, press "cmd + shift + p" and type "list gem" (or ctrl + shift + p if you're on Windows or Linux)
* Once you see "Gem Browser: List Gems", press enter.
* It will list all the gems that have been installed via bundle for the project folder 
  ![ScreenShot](https://dl.dropbox.com/u/1252099/semi-permanent/gembrowser.png)
* Once you choose a gem of the list, this plugin will open the source of the gem in a new window with the code ready for inspection and EVEN modification in real time (useful for debugging).

# Installation

### Package Control
Using [Package Control](http://wbond.net/sublime_packages/package_control), a
package manager for Sublime Text.

In ST, press "cmd + shift + p" and then type "install".

Once you see "Package Control: Install Package", press enter.

When the packages load, another selection window will appear.

Type "gem browser" and enter. All done!

### Manual Installation for Sublime Text 2

```bash
  cd "~/Library/Application Support/Sublime Text 2/Packages/"
  git clone https://github.com/NaN1488/sublime-gem-browser.git
```

### Sublime Text 3 (Mac OS X only)
```bash
  cd "/Applications/Sublime Text.app/Contents/MacOS/Packages"
  curl https://github.com/NaN1488/sublime-gem-browser/archive/master.zip -o sublime-gem-browser.sublime-package
  zip -j -r sublime-gem-browser.sublime-package sublime-gem-browser/*
  rm -rf sublime-gem-browser
```

### Fix for Ruby path issues on Mac OS X

Gem Browser makes an effort to find the proper Ruby executable on your computer. However, if you still get errors such as 'could not find gem ... in any of the sources' or just Ruby not being found, you should install the [Fix Mac Path](https://github.com/int3h/SublimeFixMacPath) plugin, which makes the $PATH from your shell available in Sublime Text. (This will also fix all kinds of build tools dependent on custom $PATH.)

## Known issues / limitations
* Experimental support for Sublime Text 3 (Only in OS X with RVM)

## License
* MIT License

2012 - Created by Nahuel Sciaratta and Bruno Bonamin
