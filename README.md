# Guide  
### A collection of documentations for the most essential operations in software development  

## Index  


## Sublime Text 3 on Ubuntu [Setup and Installation]

The Ubuntu version used is 16.04, but it should be easily adapted to other Ubuntu flavors or even other Linux distros.

### Installation

```  
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -  
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list  
sudo apt update && sudo apt install -y sublime-text
```  
 
### Uninstall Sublime Text:  
`sudo apt remove sublime-text && sudo apt autoremove`

### To make Sublime shine, install Package Control to easily install plugins

- The ease one: hit `Ctrl + Shipt + P`, type `Install Package Control` and choose it to install. Wait some seconds and that's all.
- The hard one: You may get a installation script from the [Package Control](https://packagecontrol.io/installation) website to install it through the Sublime Console. Choose the script for version 3. Copy and paste in in the console and hit enter, wait a little while and you're done.

### Adding plugins

To install a plugin via Package Control, hit `Ctrl + Shift + P`, type `Install Pakcage`, and chose `Package Control: Install Package`

After a little while you should see a list of plugins available. Just type the plugin's name, choose it, wait while it gets installed and you're done

- SideBarEnhancements
- Materia design with [Box Theme](https://packagecontrol.io/packages/Boxy%20Theme).

To enable the installed theme go to `Preferences > Settings` and paste the following:

```json
{
	"color_scheme": "Packages/Boxy Theme/schemes/Boxy Ocean.tmTheme",
	"highlight_line": true,
	"rulers":
	[
		100
	],
	"theme": "Boxy Ocean.sublime-theme",
	"theme_accent_cyan": true,
	"theme_bar": true,
	"theme_bar_logo_atomized": true,
	"theme_bar_shadow_hidden": true,
	"theme_button_rounded": true,
	"theme_dirty_colored_always": true,
	"theme_icons_materialized": true,
	"theme_scrollbar_rounded": true,
	"theme_sidebar_highlight_selected_text_only": true,
	"theme_sidebar_highlight_text_only": true,
	"theme_sidebar_indent_top_level_disabled": true,
	"theme_size_md": true,
	"theme_tab_highlight_text_only": true,
	"theme_tab_selected_transparent": true,
	"theme_tab_selected_underlined": true,
	"theme_tab_size_xxl": true,
	"theme_unified": true
}
```

If you would like to see more options for themes, I recommend [this guide](https://scotch.io/bar-talk/best-sublime-text-3-themes-of-2015-and-2016)
