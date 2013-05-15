vimconfig
=========================================
Custom Vim configuration example (Windows)

Installed plugins
-----------------

* Autoclose (to close braces, quotes, etc.)
* Pathogen (plugin manager)
* Omnicppcomplete (c++ autocomplete)
* Powerline (status bar)
* NERDTree (file system tree)
* MRU (The list of recently opened files)
* snipMate (code snippets)
* session (save and restore sessions)
* T-Comment (handle code comments)
* Neosnippet (code snippets)
* Neocomplcache (autocompletion)
* TagHighlight (tags highlighting)

Setup
-----

1. Install Vim
2. Clone vimconfig and all plugins:

        git clone git://github.com/vahancho/vimconfig.git
        cd vimconfig
        git submodule init
        git submodule update

3. Create a link to the new vimfiles in vim directory. For example: 

    `mklink /D "C:\Program Files (x86)\Vim\vimfiles" "D:\projects\vimconfig\vimfiles"`

4. Create a link to the new vimrc file in vim directory. For example: 

    `mklink "C:\Program Files (x86)\Vim\_vimrc" "D:\projects\vimconfig\.vimrc"`
    
5. Create a link to the 'autoload' directory of pathogen plugin:
        
        cd <vimfiles>
        mklink /D autoload bundle\vim-pathogen\autoload

5. Install Ecuberant Ctags (http://ctags.sourceforge.net/)
6. Create tag files at tags directory. For example for Qt4:

        cd <vimfiles>    
        mkdir tags
        cd tags    
        ctags -R --sort=yes --c++-kinds=+p --fields=+iaS --extra=+q --language-force=C++ -f qt4 /usr/include/qt4/ # for QT4`

7. Generate documentation tags for all plugins with `:Helptags` command.
