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
