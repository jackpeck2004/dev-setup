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
    