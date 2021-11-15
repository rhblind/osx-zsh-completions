OSX ZSH COMPLETIONS
===================
Provides zsh completions for selected OSX commands. This repository's main
purpose is to create quality auto completions, e.g. conditional flag aware
presentation and selection of choices, as well as up-to-date and
feature-complete auto completions.

INSTALLATION
============

#### [oh-my-zsh](http://github.com/robbyrussell/oh-my-zsh)

* Clone the repository inside your oh-my-zsh repo:

        git clone https://github.com/rhblind/osx-zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/osx-zsh-completions

* Enable it in your `.zshrc` by adding it to your plugin list and reloading the completion:

        plugins=(… osx-zsh-completions)
        autoload -U compinit && compinit

#### Manual installation

* Clone the repository:

        git clone https://github.com/rhblind/osx-zsh-completions

* Include the directory in your `$fpath`, for example by adding in `~/.zshrc`:

        fpath=(path/to/osx-zsh-completions $fpath)

* You may have to force rebuild `zcompdump`:

        rm -f ~/.zcompdump; compinit

CONTRIBUTE
==========
Feel free to raise an issue. If you have already created a completion for a
particular command and would like to see it included, fork the repo and submit
a pull request, same goes for any bugs you might encounter.

**This is a work in progress...**

LICENSE
=======

Copyright (C) 2012-2014 nilsonholger@hyve.org

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
