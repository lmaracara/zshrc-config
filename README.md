# Terminal Configuration with .zshrc

This guide helps you set up your terminal using the provided `.zshrc` for a modern, productive shell experience on macOS.

## Prerequisites

Before using this configuration, install:

### 1. iTerm2
A powerful terminal emulator for macOS.  
[Download iTerm2](https://iterm2.com/)

### 2. Oh My Zsh
A popular framework for managing your Zsh configuration.  
[Oh My Zsh Installation Guide](https://ohmyz.sh/#install)

### 3. Powerlevel10k Theme
A fast, flexible, and beautiful Zsh prompt.  
[Powerlevel10k GitHub](https://github.com/romkatv/powerlevel10k)

**Install Powerlevel10k:**
```sh
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```
**Configure Powerlevel10k:**  
Set the theme in your `.zshrc`:
```sh
ZSH_THEME="powerlevel10k/powerlevel10k"
```
To customize your prompt, run:
```sh
p10k configure
```

## Plugin Installation

This configuration uses several plugins:
- `git`
- `fzf`
- `zsh-autosuggestions`
- `zsh-syntax-highlighting`
- `you-should-use`
- `zsh-bat`
- `thefuck`

**Install Plugins:**

- **fzf** ([GitHub](https://github.com/junegunn/fzf))
	```sh
	brew install fzf
	$(brew --prefix)/opt/fzf/install
	```
- **zsh-autosuggestions** ([GitHub](https://github.com/zsh-users/zsh-autosuggestions))
	```sh
	git clone https://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
	```
- **zsh-syntax-highlighting** ([GitHub](https://github.com/zsh-users/zsh-syntax-highlighting))
	```sh
	git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
	```
- **you-should-use** ([GitHub](https://github.com/MichaelAquilina/zsh-you-should-use))
	```sh
	git clone https://github.com/MichaelAquilina/zsh-you-should-use $ZSH_CUSTOM/plugins/you-should-use
	```
- **zsh-bat** ([GitHub](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/zsh-bat))
	(Included with Oh My Zsh, just add to plugins list)
- **thefuck** ([GitHub](https://github.com/nvbn/thefuck))
	```sh
	brew install thefuck
	```

## How to Use This .zshrc

1. **Backup your current .zshrc (optional):**
	 ```sh
	 mv ~/.zshrc ~/.zshrc.backup
	 ```
2. **Link the provided .zshrc:**
	 ```sh
	 ln -s <absolute_path_to_this_folder>/.zshrc ~/.zshrc
	 ```
3. **Reload your shell:**
	 ```sh
	 source ~/.zshrc
	 ```

## Additional Notes

- Customize aliases and user settings in the `.zshrc` as needed.
- For prompt customization, edit `~/.p10k.zsh` or run `p10k configure`.
- Ensure you have [Homebrew](https://brew.sh/) installed for easy plugin installation.

---
Enjoy your enhanced terminal experience!
