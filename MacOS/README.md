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

