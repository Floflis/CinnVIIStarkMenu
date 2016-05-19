# StarkMenu
A custom menu for Cinnamon based on the look of Windows 7 Menu, derived from StarkMenu@mintystark (fixed by bluedxca93).

This menu is adapted by me to look better with the CinnXP theme by petruzzi4prez.

* https://www.dropbox.com/s/lih7li11ktctsgo/CinnXPStarkMenu_1.png
* https://www.dropbox.com/s/15kod4as1nlmh54/CinnXPStarkMenu_2.png

### This applet works on:
Linux Mint 17.3 Cinnamon (Cinnamon-Version 2.8)

### Installation guide:
1. Download ZIP
2. Extract "starkmenu-master.zip"
3. Rename the extracted "starkmenu-master" folder to "CinnXPStarkMenu@NikoKrause" 
   (This step is important, otherwise the applet won't work.)
4. Move "CinnXPStarkMenu@NikoKrause" folder to path "~/.local/share/cinnamon/applets/"
5. Add applet to panel

* For German Translation replace "settings-schema.json" file with "/languages/YOURLANGUAGE/settings-schema.json" file. --> Maybe you have to delete afterwards the "CinnXPStarkMenu@NikoKrause" folder in "~/.cinnamon/configs/" and restart Cinnamon with Ctrl+Alt+Esc

### If in use with CinnXP theme by petruzzi4prez you have to make some changes:
1. Open "CinnXP/cinnamon/cinnamon.css"
2. Add the following lines and save the file:

-------------------------------------------------------------------------------------------------
```
/* ===================================================================
 * CinnXPStarkMenu 
 * (if CinnXPStarkMenu is used, change some stuff, else use default)
 * ===================================================================*/
.starkhover-box {
	background-color: #D3E5FA; /* change background, of the box
                                      with user name and icon */
}
.starkhover-label{
	color : #000; /* change color of user name font */
}
.starkmenu-background {
	padding: 54px 1px 30px 1px;
}
.starkmenu-selected-app-box {
    color: black; /* Information, which is shown, if you select apps*/
}
.starkmenu-favorites-box {  
        background-color: white;
    border: 0px solid white;
    padding-bottom: 0.3em; /* prevent button "All Programs" and "Favorites" from jumping */
}
.starkmenu-favorites-box:spacing-shutdown-dropdown {  
    spacing: 12px; /* fix jumping and spacing issues of shutdown menu */
}
.starkmenu-favorites-box:spacing-shutdown-classic {  
    spacing: 7px; /* fix jumping and spacing issues of shutdown menu */
}
.starkmenu-applications-box {
    padding: 0px 0px 0px 0px;
    background-color: #D3E5FA;
}
.starkmenu-applications-box StScrollView {
    border-right-width: 1px;
    border-bottom-width: 1px;
    background-color: #ece9d8;
    color: black;
}
```
-------------------------------------------------------------------------------------------------

###### ToDo and Bugs (help and hints are welcome):
* Find a better way to translate the settings-schema.json file
* [Minor Bug] After removing favorite with largest name, the favorites box should resize while menu is still open, but it doesn't.