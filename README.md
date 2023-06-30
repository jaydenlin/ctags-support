# [CTags Support](https://github.com/jaydenlin/ctags-support) 
> An extension that provides `CTags Support` in [Visual Studio Code](https://code.visualstudio.com/)!
```
ext install ctags-support
```

## Additional Setup
You have to install [CTags](http://ctags.sourceforge.net/) and generate the .tags file before you use this extension.
Run the CTags command under the your project folder.
```
ctags -R -f .tags
```

## Keybinding
### 1. Navigate to Defination
Select the words in the vscode and the press `cmd+t` (`ctrl+t`)  
![IDE](https://i.giphy.com/3oEjHLg2xzc5ZS2kEg.gif) 

### 2. See Navigation History
Press `cmd+shift+t` (`ctrl+shift+t`)  
![IDE](https://i.giphy.com/l0MYrSdrYUJ8Q6BJS.gif) 

## Other Features
### 1. Clear All Navigation History
Press `f1` and input `Ctags Support: clear all navigation history`  
![IDE](https://i.giphy.com/l0MYIXWMJpUvyzTmE.gif) 

### 2. Clear One Navigation History
Press `f1` and input `Ctags Support: clear one navigation history`, then choose the one you would like to delete    
![IDE](https://i.giphy.com/l46CthKXDTO9DFQFW.gif) 

## Custom Keybinding
You can also set custom shortcuts in `keybindings.json` via `Code => Preferences => Keyboard Shortcuts`  
For example:  
`Navigate to Defination`
```
[
    { "key": "cmd+t",//set to your favorite shortcut
      "command": "extension.searchTags",
      "when": "editorTextFocus" }
]
```
`See Navigation History`  
```
[
    { "key": "cmd+shift+t",//set to your favorite shortcut
      "command": "extension.showNavigationHistory",
      "when": "editorTextFocus" }
]
```
`Clear All Navigation History`  
```
[
    { "key": "set to your favorite shortcut",//set to your favorite shortcut
      "command": "extension.clearAllNavigationHistory",
      "when": "editorTextFocus" }
]
```
`Clear One Navigation History`  
```
[
    { "key": "set to your favorite shortcut",//set to your favorite shortcut
      "command": "extension.clearOneNavigationHistory",
      "when": "editorTextFocus" }
]
```

## Issues
Please submit issues to [ctags-support](https://github.com/jaydenlin/ctags-support)

**Enjoy!**
