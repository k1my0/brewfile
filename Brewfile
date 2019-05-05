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

  ## Terminal Multiplexer
  # Terminal multiplexer with VT100/ANSI terminal emulation
  brew 'screen'
  # A terminal multiplexer, allowing to access multiple separate terminal sessions
  brew 'tmux'
  # Reattach process (e.g., tmux) to background
  brew 'reattach-to-user-namespace'

  ## Shell: Fish
  # User-friendly command-line shell for UNIX-like operating systems
  # INFO: Need to add `/user/local/bin/fish` to `/etc/shells`
  brew 'fish'
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
  # r installation
  # Using coatless professor method for OpenMP
  # https://github.com/sethrfore/homebrew-r-srf
  # reference : https://luispuerto.net/blog/2018/05/11/installing-r-with-homebrew-with-all-the-capabilities/
  # https://discourse.brew.sh/t/r-installs-on-high-sierra-without-tcl-tk-support/1190/17
  
  tap 'sethrfore/homebrew-r-srf'

  # to develop a version of the X.org x window system that runs on os X
  cask 'xquartz'
  
  # Need Command: sudo installer -pkg /Library/Developer/CommandLineTools/Packages/macOS_SDK_headers_for_macOS_10.14.pkg -target /
 
  # cairo: a 2d graphics library with support for multiple output devices
  # brew 'sethrfore/r-srf/cairo'

  brew 'sethrfore/r-srf/r', args: ['with-libtiff', 'with-openblas', 'with-java', 'with-pango']

  # r-stutio
  cask 'rstudio'
### }}}
