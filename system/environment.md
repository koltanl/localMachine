# Arch Environment Context

## System Overview
- **OS**: Arch Linux (rolling release)
- **Desktop Environment**: KDE Plasma (primary), sometimes Hyprland
- **Display Server**: Wayland (wayland-0)
- **Session Type**: wayland
- **Shell**: zsh (/bin/zsh)

## Shell Configuration
- **RC File**: ~/.zshrc (comprehensive setup with plugins)
- **Editor**: micro (export EDITOR=micro)
- **Plugins**: 
  - zsh-autosuggestions
  - zsh-syntax-highlighting
  - fzf (key bindings + completion)
- **Tools**: 
  - oh-my-posh (prompt theme from ~/.config/omp.json)
  - zoxide (smart cd with alias cd='z')
  - atuin (shell history sync)
  - fastfetch (system info on shell start)

## Terminal
- **Primary**: Kitty
- **Config**: ~/.config/kitty/kitty.conf
- **Font**: MesloLGS NF
- **Features**: 
  - Remote control enabled (unix:/tmp/kitty)
  - Background image support
  - Font scaling (ctrl+=/-)

## File Manager
- **Primary**: nnn
- **Config**: ~/.config/nnn/
- **Opener**: ~/bin/nnn_opener.sh
- **Terminal**: kitty
- **Plugins**: preview-tui, fzcd

## Development Tools
- **Neovim**: /sbin/nvim (v0.11.4) - likely lazyvim setup
- **Go**: ~/.config/go/ (Go development)
- **Package Manager**: yay (AUR helper) - ~/.config/yay/

## Key Paths
- **Binaries**: ~/bin, ~/.local/bin, ~/go/bin
- **Config**: ~/.config/
- **Cache**: ~/.cache/zsh/$HOST
- **Local IP**: Auto-detected and exported as $LOCAL_IP

## Environment Variables
- **TERM**: xterm-256color
- **PAGER**: moar (with auto-detection fallback to less/more)
- **NNN_TERMINAL**: kitty
- **STARTUP_TIMER**: true (shows shell startup time)

## Desktop Environment Details
- **Current**: KDE Plasma (wayland session)
- **Display Manager**: SDDM
- **Session**: startplasma-wayland
- **Alternative**: Hyprland (when not using KDE)
