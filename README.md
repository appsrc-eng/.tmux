# tmux config

This is a simple but useful setup for tmux, it will continue to grow overtime as more...


### Plugin Inventory

- [tmux-plugins/tpm](https://github.com/tmux-plugins/tpm)
  - tpm refers to the TPM (Tmux Plugin Manager) that is a part of the tmux-plugins project. This plugin manager is designed to handle the installation, loading, and management of other tmux plugins. tmux is a terminal multiplexer, which allows multiple terminal sessions to be accessed and controlled from a single screen.
  - tpm simplifies the process of adding plugins to tmux, managing their configuration, and updating them when new versions are released.

- [tmux-plugins/tmux-sensible](https://github.com/tmux-plugins/tmux-sensible)
  - tmux-sensible is a plugin within the tmux-plugins collection, and it’s designed to provide a set of sensible default configurations for tmux. The goal of this plugin is to make tmux more user-friendly and usable out of the box, without requiring extensive customization and configuration.
  - tmux-sensible provides a range of default settings that are considered to be universally acceptable and beneficial to most tmux users. These may include settings related to:
    - terminal behavior and appearance
    - window and pane configurations
    - key bindings
    - other basic tmux settings

- [christoomey/vim-tmux-navigator](https://github.com/christoomey/vim-tmux-navigator)
  - vim-tmux-navigator allows seamless navigation between Vim splits and tmux panes. This means that if you use Vim as your text editor within a tmux session, this plugin provides a consistent way to navigate across both Vim splits and tmux panes using the same key bindings.
  - Features: 
    - allows users to navigate between Vim splits and tmux panes using a consistent set of key bindings.
    - convenient for users who frequently work with tmux and Vim together, as it makes the process of navigating between different panes and splits more efficient and intuitive.

- [dracula/tmux](https://github.com/dracula/tmux)
  - dracula is a theme for tmux, provided by the Dracula Theme project. The Dracula Theme is a popular color scheme used in various applications, tools, and environments to provide a specific aesthetic that includes a dark background and vibrant foreground colors.
  - Features: 
    - dark theme: It provides a dark color palette, which can be easier on the eyes and is preferred by many users, especially when working in low-light conditions.
    - vibrant colors: The theme uses vibrant colors to highlight different elements on the screen, making it easier to differentiate between them.


### Tmux Plugin Manager (TPM) Installation + Custom Config

1) Validate requirements
    - tmux version 1.9 (or higher)
    - git
    - bash

2)  Clone the `tmux-plugins/tpm` repo to the specified directory
```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

3) Move the `.tmux.conf` file from this repo to `~/.tmux.conf`<br><br /> 

4) Reload TMUX environment so TPM is sourced
```bash
# type this in terminal if tmux is already running
tmux source ~/.tmux.conf
```