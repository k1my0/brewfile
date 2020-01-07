# Brewfile
#
# Maintained by Hyojin Kim <cti.hyooo@gmail.com>
# http://www.hyooojin.kim/


cask_args appdir: '/Applications'

# Install and manage GUI macOS applications
tap 'homebrew/cask'
# Alternative versions of Casks
tap 'homebrew/cask-versions'
# Integrates Homebrew formulae with macOS' `launchctl` manager
tap 'homebrew/services'
# A CLI tool upgrading every outdated app installed by Homebrew Cask
# INFO: brew cu
tap 'buo/cask-upgrade'


### Web {{{
  ## Web Browser
  cask 'firefox-developer-edition'

  ## Flash Player for Web Browser
  # Adobe Flash Player NPAPI (plugin for Safari and Firefox)
  cask 'flash-npapi'
  # Adobe Flash Player PPAPI (plugin for Opera and Chromium)
  cask 'flash-ppapi'
### }}}


### Messaging {{{
  cask 'slack'
  cask 'telegram'
### }}}


### Keyboard & Mouse {{{
  # Know your shortcuts
  cask 'cheatsheet'
### }}}


### Terminal {{{
  ## Terminal Emulator
  # Terminal Emulator for macOS
  cask 'iterm2'
  # https://github.com/mbadolato/iTerm2-Color-Schemes/blob/master/schemes/Snazzy.itermcolors
  # UNIX shell (command interpreter)
  brew 'zsh'
  brew 'zsh-completions'

  ## Terminal Multiplexer
  # Terminal multiplexer with VT100/ANSI terminal emulation
  brew 'screen'
  # A terminal multiplexer, allowing to access multiple separate terminal sessions
  brew 'tmux'
  # Reattach process (e.g., tmux) to background
  brew 'reattach-to-user-namespace'
  

  # Ambitious Vim-fork focused on extensibility and agility
  brew 'neovim'
  tap 'homebrew/cask-fonts'
  cask 'font-hack-nerd-font'
  

  ## Shell: Fish
  # User-friendly command-line shell for UNIX-like operating systems
  # INFO: Need to add `/user/local/bin/fish` to `/etc/shells`
  brew 'fish'

  # Command-line fuzzy finder written in Go
  brew 'fzf'

  # CLI tool for quick access to files and directories
  brew 'fasd'

  # docker
  brew 'docker'

  # nmap
  brew 'nmap'
  # fping
  brew 'fping'
### }}}

### Database {{{
  ## SQL
  # SQLite
  brew 'sqlite'
  # MySQL
  brew 'mysql'
### }}}

### Code Editor & IDE {{{
  ## Editor: Sublime Text
  cask 'sublime-text'

  ## Editor: Visual Studio
  cask 'visual-studio-code'

  ## Editor: Typora
  #  cask 'typora'

  ## Editor: Boostnote
  cask 'boostnote' 
### }}}

### Virtualization {{{
  ## Container
  # Docker Community Edition for Mac (Edge)
  cask 'docker-edge'
  # Kubernetes command-line interface
  brew 'kubernetes-cli'
### }}}


### Development {{{
  # Automatic configure script builder
  brew 'autoconf'
  # Tool for generating GNU Standards-compliant Makefiles
  brew 'automake'
  # Cross-platform make
  brew 'cmake'
  # Trello
  # cask 'trello-x'
  #  Git
  brew 'git'
  brew 'git-flow'
  brew 'git-lfs'
### }}}


### Programming Language {{{
  ## Python
  # Python3
  brew 'python'
  # Python2
  brew 'python@2'
  # Python dependency management tool
  brew 'pipenv'

  ## Java
  cask 'java'

  ## R
  cask 'r'
  # r-stutio
  cask 'rstudio'

  ## nodejs
  brew 'nodejs'

  ## ruby
  brew 'ruby'
  brew 'rbenv'
  brew 'ruby-build'
### }}}
