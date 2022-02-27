# MacOS
## Procedure
### Pre-requisites
- [Homebrew](https://brew.sh)

## Commands
```bash
xcode-select --install
wget https://raw.githubusercontent.com/jackpeck2004/dev-setup/main/MacOS/Brewfile
brew bundle
```
## Configurations
- iTerm2:
    - Apperance > General > Theme = Minimal
    - Download iTerm2 theme (Theme.json)
    	- ```wget https://raw.githubusercontent.com/jackpeck2004/dev-setup/main/MacOS/Theme.json```
    - Download iTerm2 keybindings (TermKeys.itermkeymap)
    	- ```wget https://raw.githubusercontent.com/jackpeck2004/dev-setup/main/MacOS/TermKeys.itermkeybindings```
    - Profiles > ... > Import JSON Profiles > Theme.json
    - Profiles > ... > (select imported theme) Set as Default
    - Keys > KeyBindings > ... Presets > Import > TermKeys.itermkeymap

- NodeJs
    - Install node v16 from fnm
        - ``` fnm install 16 ```

- System Preferences
    - Keyboard > Shortcuts > Keyboard > Move focus to Next Window = alt + tab
    - Download settings sh script
        - ```wget https://raw.githubusercontent.com/jackpeck2004/dev-setup/main/MacOS/settings-setup.sh```
    - ```chmod a+x settings-setup.sh```
    - ```./settings-setup.sh```

- Rectangle
    - Download config ```wget https://raw.githubusercontent.com/jackpeck2004/dev-setup/main/MacOS/RectangleConfig.json```
    - Rectangle > Preferences > "Gear Icon" > Import > RectangleConfig.json

- ZSH
```bash
wget https://raw.githubusercontent.com/jackpeck2004/dev-setup/main/MacOS/zshrc > ~/.zshrc
wget https://raw.githubusercontent.com/jackpeck2004/dev-setup/main/MacOS/p10k > ~/.p10k.zsh
source ~/.zshrc
mkdir ~/.config
curl https://gist.githubusercontent.com/jackpeck2004/542c68823c13fd10ab9601623be1730d/raw/e1b81eee300371bf340997171322056e732ec9d6/alias > ~/.config/alias

```
- Neovim
```bash
mkdir ~/.config/nvim
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
curl https://gist.githubusercontent.com/jackpeck2004/3ddf25c7166e904d57a9bddf36d2f2db/raw/2d9aff38634368f282228e16d86c650c3a01acc8/init.vim > ~/.config/nvim/init.vim
```
- TMUX
```bash
curl https://gist.githubusercontent.com/jackpeck2004/5c99b4d4bc6048d56fe66ce559d76a47/raw/2a4ccb75e3358e22c8b4ac4115e8adcdb21ab163/tmux-conf > ~/.tmux.conf
```