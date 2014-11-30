# About
This repository contains configuration files I use on Mac and Linux systems
which have been inspired by the rest of the dotfiles community.
This `README` has been automatically generated by
[generate-readme.sh][generate-readme.sh] on Sun Nov 30 13:57:41 EST 2014.
The following screenshots are automatically generated by
the [screenshots/generate.sh][screenshot-gen] script
by taking screenshots in an [X virtual framebuffer][xvfb].

[screenshot-gen]: https://github.com/bamos/dotfiles/blob/master/screenshots/generate.sh
[xvfb]: http://www.x.org/archive/X11R7.7/doc/man/man1/Xvfb.1.xhtml
[generate-readme.sh]: https://github.com/bamos/dotfiles/blob/master/generate-readme.sh
## vim
![](https://raw.githubusercontent.com/bamos/dotfiles/master/screenshots/vim.png)
## emacs
![](https://raw.githubusercontent.com/bamos/dotfiles/master/screenshots/emacs.png)
## zsh
![](https://raw.githubusercontent.com/bamos/dotfiles/master/screenshots/zsh.png)
## mutt
![](https://raw.githubusercontent.com/bamos/dotfiles/master/screenshots/mutt.png)
## screen
![](https://raw.githubusercontent.com/bamos/dotfiles/master/screenshots/screen.png)
## tmux
![](https://raw.githubusercontent.com/bamos/dotfiles/master/screenshots/tmux.png)
# Installation

Use [bootstrap.sh][bootstrap.sh] to symlink all of the dotfiles
in this repo to the home directory and install vim plugins.
An alternate to manually linking with shell script is to use [GNU Stow][stow].
I'm keeping the shell script for now because some machines
I have non-sudo access to don't have GNU Stow installed.

```Bash
git clone --recursive git://github.com/bamos/dotfiles.git .dotfiles
cd .dotfiles
./bootstrap.sh
```

[bootstrap.sh]: https://github.com/bamos/dotfiles/blob/master/bootstrap.sh
[stow]: http://www.gnu.org/software/stow/


# Shell functions and aliases.
The following is a summary of custom Bash and zsh functions and
aliases contained in [.funcs][funcs] and [.aliases][aliases].

[funcs]: https://github.com/bamos/dotfiles/blob/master/.funcs
[aliases]: https://github.com/bamos/dotfiles/blob/master/.aliases

## Functions
+ die
+ rand-cd
+ wget-rec
+ d2h
+ mkdircd
+ nj
+ musicToAndroid
+ docker-clean
+ docker-zsh
+ ps-threads
+ watch-threads
+ crontab
+ inf
+ memo
+ lapack-install
+ function stopwatch
+ git-dirty
+ git-clonecd
+ sys-find
+ dump-packages

## Aliases
| Alias | Definition |
|---|---|
.. | 'cd ..'
... | 'cd ../..'
.... | 'cd ../../..'
..... | 'cd ../../../..'
...... | 'cd ../../../../..'
acs | 'apt-cache search'
add-tags | 'picard'
agi | '_ apt-get install -y'
agr | '_ apt-get remove -y'
aup | '_ apt-get update; _ apt-get upgrade;'
bcl | 'vim +BundleClean +qall'
bri | 'brew install'
brun | 'brew uninstall'
brup | 'brew update; brew upgrade'
bup | 'vim +BundleInstall +qall'
c | 'clear'
chax | 'chmod a+x'
chromium | 'chromium-browser'
count-frames | $'grep -c \'^\\(\\\\frame{\\|\\\\begin{frame}\\\)\''
dual | 'xrandr --output VGA1 --right-of LVDS1 --auto'
dx | 'dual; exit'
emacs | "$HOME/Applications/Emacs.app/Contents/MacOS/Emacs"
emacs | 'emacsclient -a "" -c'
emacsn | "$HOME/Applications/Emacs.app/Contents/MacOS/Emacs -nw"
emacsn | '\emacs -nw'
f | 'sudo $(fc -ln -1)'
g | 'git'
ga | 'git add'
gc | 'git commit'
gclo | 'git clone'
gcloc | 'git-clonecd'
get-tags | 'exiftool -json'
gl | 'git pull'
gp | 'git push'
gpsuom | 'git push --set-upstream origin master'
grive | 'grive -p ~/grive'
gsd | 'git svn dcommit'
gsr | 'git svn rebase'
gu | "git reset --soft 'HEAD^'"
h | 'hostname'
i-ext | 'curl icanhazip.com'
i-int | 'ip address show wlp3s0'
i-int | 'ipconfig getifaddr en0'
less | '/usr/local/Cellar/macvim/7.4-73/MacVim.app/Contents/Resources/vim/runtime/macros/less.sh'
less | '/usr/share/vim/vim74/macros/less.sh'
li | 'libreoffice'
m | 'make -j8'
m2a | 'musicToAndroid'
mcd | 'mkdircd'
mu | 'mutt'
psg | 'ps aux | grep'
pullimages | "adb pull /storage/sdcard0/DCIM/Camera ."
pw | 'pwgen --numerals --symbols --ambiguous 15 1'
rcd | 'rand-cd'
remove-tags | 'eyeD3 --remove-all'
rh | 'rehash'
rsyncdir | 'rsync -azv --progress'
sudo | 'nocorrect sudo'
sync-music | 'rsyncdir $HOME/docs/music/ dijkstra:~/mnt/usb/music/'
tmux | 'tmux -2'
up | 'yaourt -Syua'
vim | 'mvim -v -p'
vim | 'vim -p'
xa | 'xrandr --auto'
xax | 'xrandr --auto; exit'
y | 'yaourt'
yr | 'yaourt -R --noconfirm'
ys | 'yaourt -S --noconfirm'
yup | 'up --noconfirm'
za | 'Skim'
za | 'zathura'
# Similar Projects and Inspiration
There are many approaches to managing dotfiles on GitHub
that have inspired this repository, and this project
uniquely adds automatic screenshot generation.
The following list was generated on 2014-11-30 and
shows a subset of related projects.
[The dotfiles page on the Arch Linux Wiki](https://wiki.archlinux.org/index.php/Dotfiles)
is another good resource.
Name | Stargazers | Description
----|----|----
[cowboy/dotfiles](https://github.com/cowboy/dotfiles) | 688 | My OS X / Ubuntu dotfiles.
[garybernhardt/dotfiles](https://github.com/garybernhardt/dotfiles) | 938 | ~grb. Things in here are often interdependent. A lot of stuff relies on scripts in bin/.
[gf3/dotfiles](https://github.com/gf3/dotfiles) | 601 | My dotfiles
[holman/dotfiles](https://github.com/holman/dotfiles) | 2716 | @holman does dotfiles
[joedicastro/dotfiles](https://github.com/joedicastro/dotfiles) | 444 | My .dotfiles
[justone/dotfiles](https://github.com/justone/dotfiles) | 127 | Dotfiles
[mathiasbynens/dotfiles](https://github.com/mathiasbynens/dotfiles) | 10126 | .files, including ~/.osx — sensible hacker defaults for OS X
[nelstrom/dotfiles](https://github.com/nelstrom/dotfiles) | 234 | My dotfiles. Mainly customisations for Vim and Bash.
[ocodo/emacs.d](https://github.com/ocodo/emacs.d) | 18 | My emacs.d
[paulmillr/dotfiles](https://github.com/paulmillr/dotfiles) | 313 | Colourful & robust OS X / \*nix configuration files and utilities. 
[pengwynn/dotfiles](https://github.com/pengwynn/dotfiles) | 253 | $HOME sweet ~/
[rmm5t/dotfiles](https://github.com/rmm5t/dotfiles) | 264 | Ryan McGeary's configuration shiznit that makes him productive
[robbyrussell/oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) | 20006 | A community-driven framework for managing your zsh configuration. Includes 120+ optional plugins (rails, git, OSX, hub, capistrano, brew, ant, macports, etc), over 120 themes to spice up your morning, and an auto-update tool so that makes it easy to keep up with the latest updates from the community.
[ryanb/dotfiles](https://github.com/ryanb/dotfiles) | 1779 | config files for zsh, bash, completions, gem, git, irb, rails
[skwp/dotfiles](https://github.com/skwp/dotfiles) | 3231 | YADR - The best vim,git,zsh plugins and the cleanest vimrc you've ever seen
[sontek/dotfiles](https://github.com/sontek/dotfiles) | 444 | My configuration files (.screenrc, .vimrc, .weechat, .bashrc, .gitconfig, etc)
[spf13/spf13-vim](https://github.com/spf13/spf13-vim) | 4060 | The ultimate vim distribution
[ssaunier/dotfiles](https://github.com/ssaunier/dotfiles) | 4 | Dot files for my macbook setup (shell = zsh)
[terhechte/emacs.d](https://github.com/terhechte/emacs.d) | 36 | My emacs.d
[thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles) | 1838 | A set of vim, zsh, git, and tmux configuration files.
[tpope/tpope](https://github.com/tpope/tpope) | 190 | tpope's dotfiles. here be dragons
[vicfryzel/xmonad-config](https://github.com/vicfryzel/xmonad-config) | 207 | My xmonad and xmobar configuration, plus necessary scripts to make things more usable.
[windelicato/dotfiles](https://github.com/windelicato/dotfiles) | 445 | arch linux configuration files
