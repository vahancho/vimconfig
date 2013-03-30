vimconfig
=========================================
Custom Vim configuration example (Windows)

Installed plugins
-----------------

* Autoclose (to close braces, quotes, etc.)
* Pathogen (plugin manager)
* Omnicppcomplete (c++ autocomplete)
* Powerline (status bar)
* NERDTree (File system tree)
* MRU (The list of recently opened files)

Installation
------------

1. Install Vim
2. Clone vimconfig (git clone git://github.com/vahancho/vimconfig.git)
3. Create a link to our custom vimfiles in vim directory directory. For example: 

    'mklink /D "C:\Program Files (x86)\Vim\vimfiles" "D:\projects\vimconfig\vimfiles"'

4. Create a link to our custom vimrc file in vim directory. For example: 

    'mklink "C:\Program Files (x86)\Vim\_vimrc" "D:\projects\vimconfig\.vimrc"'

5. Install Ecuberant Ctags (http://ctags.sourceforge.net/)

