# Introduction
## Installation
### oh-my-posh
This is for changing Themes. You can install it on the [Microsoft Store](https://apps.microsoft.com/detail/xp8k0hkjfrxgck?mode=mini). For further information see the [oh-my-posh Website](https://ohmyposh.dev/docs/installation/windows).


### Fonts
oh-my-posh works with Nerd Fonts, which are popular fonts that are patched to include icons. You can install this with `oh-my-posh font install`. This will present a list of Nerd Font libraries, from which you can select one. I recommend the **Meslo** front.

Afetwards you have to configure your Terminal to use that font. Go into your Terminal settings with `CTRL + SHIFT + ,`. This will open the settings.json. Now add the `font.face` attribute under the `defaults` attribute in `profiles`:
```
{
    "profiles":
    {
        "defaults":
        {
            "font":
            {
                "face": "MesloLGM Nerd Font"
            }
        }
    }
}
```
*For more information see https://ohmyposh.dev/docs/installation/fonts*

### $PROFILE
Use `notepad $PROFILe` to open the PowerShell Profile. If it doesen't exist, this command will create it.

Now you can finaly paste the contents of the $PROFILE file of the Repository into your $PROFILE.

## Commands

### Theme
Use `Theme <Theme Name>` to activate one of the predefined Themes. You can edit this in your $PROFILE by editing the themeMap. For example this `"cloud1" = "cloud-native-azure"` means you can type `Theme cloud1` to activate the `cloud-native-azure` Theme, which is a oh-my-posh Theme.

You can see all the themes with `Get-ChildItem -Path "~/.poshthemes" -Filter "*.omp.json"`. Here you can also edit or add Themes. 

*For more information see https://ohmyposh.dev/docs/configuration/general*

### time
Use `time` to see the Current time *(I was bored)*.

### work
Use `work` to go to **C:\work**.

