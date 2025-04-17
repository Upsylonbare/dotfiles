# Dotfiles

This repository contains my personal configuration files (dotfiles) for various tools and applications. The setup is managed using [GNU Stow](https://www.gnu.org/software/stow/), which simplifies the process of symlinking configuration files to their appropriate locations.

## Structure

Each directory in this repository corresponds to a specific application or tool. For example:
- `starship/` contains configuration files for Starship prompt.
- `vscode/` contains configuration files for Visual Studio Code.
- `zsh/` contains configuration files for Zsh.
- `git/` contains configuration files for Git.

## Installation

1. Clone this repository to your home directory or a preferred location:
    ```bash
    git clone https://github.com/Upsylonbare/dotfiles.git ~/.dotfiles
    ```

2. Navigate to the repository:
    ```bash
    cd ~/.dotfiles
    ```

3. Use `stow` to symlink the desired configuration. For example, to set up Zsh:
    ```bash
    stow zsh
    ```

    This will create symlinks for the Vim configuration files in your home directory.

4. Repeat the `stow` command for other configurations as needed:
    ```bash
    stow zsh
    stow git
    ```

## Adding New Configurations

1. Create a new directory in the repository for the application/tool.
2. Place the configuration files in the new directory, maintaining the same structure as they would appear in your home directory.
3. Use `stow` to symlink the new configuration.

## Uninstalling Configurations

To remove symlinks created by `stow`, use the `-D` option. For example: