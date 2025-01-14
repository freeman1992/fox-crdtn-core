# CRDTN Core

A client/server side mod which is a foundation for my other mods. It's a simple package with various functions that can be used across multiple mods and server owners can benefit from those in their custom mods. Server side mod is not required. You can also use this mod as allows server owners extend their game experience by adding my notification UI and custom sounds. 

For those who are not very familiar with scripting, I would suggest to take a look on the documentation or join my discord and ask for help. It's a nice simple mod which can help you to get things sorted out and maybe understand better how to structure a simple mod. 

This mod is important for the other CRDTN mods to get things organized and consistent so please be aware that repacking of this mod does not bring you any benefit. Rather visit a public github repository with a source code and do some study or read the docs. 

## Features in nutshell: 

- Rest Api Wrapper [https://dayz.foxapo.com/mods/crdtn-core/rest-api]
- File Logger [https://dayz.foxapo.com/mods/crdtn-core/file-logger]
- Event handler [https://dayz.foxapo.com/mods/crdtn-core/event-handler]
- Notifications UI [https://dayz.foxapo.com/mods/crdtn-core/notifications-ui]
- Sound upon login to game 
- Generic UI List Entry and UI Menu
- [TODO] Preparation of Post Processing requester
- [TODO] Preparation of Camera utility class for easier manipulation with camera
- [TODO] Support for Discord hooks

### Config $profiles/CRDTN/CRDTN_Core.json
```json
{
    "CRDTN_ServerName": ">> SERVER NAME <<",
    "CRDTN_IntroSoundSet": "CRDTN_SoundSet_StalkerSounds_Ambient_09",
    "CRDTN_NotificationsWrapper": "CRDTN_Core/Layouts/Notifications/notifications.layout",
    "CRDTN_Notifications": "CRDTN_Core/Layouts/Notifications/notification_element.layout",
    "CRDTN_UseVanillaNotifications": 0,
    "CRDTN_DisableIntroNotification": 0,
    "CRDTN_Debug": 1,
    "CRDTN_IntroMusic": 1,
    "CRDTN_AdminList": [
        "avCdzuTN2GEbHlqfPk2wXFvUyxW7CVe50bFIWgDCvN0="
    ],
    "CRDTN_Packages": {
        "COMMENT": "HERE COMES THE URLS FOR THE APIs - For example: http://localhost:9999/api",
        "service-api": "endpoint"
    }
}
```

- If you don't like the notification look & feel, you can always use the vanilla notifications by putting the following value in the config to **CRDTN_Notifications** parameter
```
gui/layouts/new_ui/notifications/notification_element.layout
```

### Usable sound sets 

You can use various Sound Sets from the mod which are licenced or aquired songs with permission from their respective authors. Please bare in mind that commercial usage of these sound effects is strictly prohibited so before you want to use this song in your mod, please raise a support ticket on my discord and we can allow you to use it. There is no need to steal this thing and do it without a permission. Some songs are used from the bought asset packs for Unity and some are acquired with the permission from Good Malware or Magnality. Both authors are members of my discord channel so if you want to contact them, do not hesitate to join the discord and write them a message. 

```
- Stalker Sounds 

    CRDTN_SoundSet_StalkerSounds_Pda_Alarm
    CRDTN_SoundSet_StalkerSounds_Pda_Communication_Lost
    CRDTN_SoundSet_StalkerSounds_Pda_Guide_2
    CRDTN_SoundSet_StalkerSounds_Pda_News 
    CRDTN_SoundSet_StalkerSounds_Pda_Objective 
    CRDTN_SoundSet_StalkerSounds_Pda_Tip
    CRDTN_SoundSet_StalkerSounds_Pda_Welcome
    CRDTN_SoundSet_StalkerSounds_Pda_Spot_Discovered

- Various ambient noises 

    CRDTN_SoundSet_StalkerSounds_Ambient_01
    CRDTN_SoundSet_StalkerSounds_Ambient_02
    CRDTN_SoundSet_StalkerSounds_Ambient_03
    CRDTN_SoundSet_StalkerSounds_Ambient_04
    CRDTN_SoundSet_StalkerSounds_Ambient_05
    CRDTN_SoundSet_StalkerSounds_Ambient_06
    CRDTN_SoundSet_StalkerSounds_Ambient_07
    CRDTN_SoundSet_StalkerSounds_Ambient_08
    CRDTN_SoundSet_StalkerSounds_Ambient_09
    CRDTN_SoundSet_StalkerSounds_Ambient_10
    CRDTN_SoundSet_StalkerSounds_Ambient_11
    CRDTN_SoundSet_StalkerSounds_Ambient_12
    CRDTN_SoundSet_StalkerSounds_Ambient_13
    CRDTN_SoundSet_StalkerSounds_Ambient_14
    CRDTN_SoundSet_StalkerSounds_Ambient_15
    CRDTN_SoundSet_StalkerSounds_Ambient_16
    CRDTN_SoundSet_StalkerSounds_Ambient_17
    CRDTN_SoundSet_StalkerSounds_Ambient_18
    CRDTN_SoundSet_StalkerSounds_Ambient_19
    CRDTN_SoundSet_StalkerSounds_Ambient_20

- Alarm sound

    CRDTN_Core_SoundSet_Sound_Alarm

- Music 

    CRDTN_Core_SoundSet_Music_Zone
    CRDTN_Core_SoundSet_Music_InvisibleThreat
    CRDTN_Core_SoundSet_Music_Oxido
    CRDTN_Core_SoundSet_Music_Tension1
    CRDTN_Core_SoundSet_Music_Tension2
    CRDTN_Core_SoundSet_Music_OldOne
```

### Usable font

If you like the fond of CRDTN mods, you can search for **Rajdhani** or use following variants of font: 
```
// Light
CRDTN_Core/data/fonts/Rajdhani-Light/Rajdhani-Light
CRDTN_Core/data/fonts/Rajdhani-Light/Rajdhani-Light16
CRDTN_Core/data/fonts/Rajdhani-Light/Rajdhani-Light20
CRDTN_Core/data/fonts/Rajdhani-Light/Rajdhani-Light22
CRDTN_Core/data/fonts/Rajdhani-Light/Rajdhani-Light24
CRDTN_Core/data/fonts/Rajdhani-Light/Rajdhani-Light26
CRDTN_Core/data/fonts/Rajdhani-Light/Rajdhani-Light28
// Medium
CRDTN_Core/data/fonts/Rajdhani-Medium/Rajdhani-Medium12
CRDTN_Core/Data/fonts/Bender/Bender-Regular14
CRDTN_Core/Data/fonts/Bender/Bender-Regular16
CRDTN_Core/Data/fonts/Bender/Bender-Regular20
CRDTN_Core/Data/fonts/Bender/Bender-Regular22
CRDTN_Core/Data/fonts/Bender/Bender-Regular48
CRDTN_Core/data/fonts/Rajdhani-Medium/Rajdhani-Medium58
// Bold
CRDTN_Core/data/fonts/Rajdhani-Bold/Rajdhani-Bold12
CRDTN_Core/data/fonts/Rajdhani-Bold/Rajdhani-Bold14
CRDTN_Core/data/fonts/Rajdhani-Bold/Rajdhani-Bold16
CRDTN_Core/Data/fonts/Bender/Bender-Regular22
CRDTN_Core/data/fonts/Rajdhani-Bold/Rajdhani-Bold28
CRDTN_Core/data/fonts/Rajdhani-Bold/Rajdhani-Bold48
CRDTN_Core/data/fonts/Rajdhani-Bold/Rajdhani-Bold58
```

**Documentation** **https://dayz.foxapo.com/mods/crdtn-core**

Thank you for checking out my Mod. Creating and maintaining mods takes time and effort, but I enjoy every moment of it. If you've found my Mod useful, entertaining, or it has enhanced your gaming experience in any way, and you feel inclined to support my work, I would sincerely appreciate any contribution you can make.

Donations are completely optional and not expected, but they do go a long way in helping me continue developing and improving this Mod. Your generosity enables me to invest more time and resources into creating new features, fixing bugs, and providing ongoing support to the community.

If you're interested in making a donation, you can find a link below. Every contribution, no matter the size, is highly valued and gratefully received. Your support means a lot to me, and it motivates me to keep pushing the boundaries of what's possible.

Thank you for considering a donation, and thank you for being a part of this amazing community. Happy gaming!

<a href="https://www.buymeacoffee.com/foxapogames"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a pizza&emoji=🍕&slug=foxapogames&button_colour=43559d&font_colour=ffffff&font_family=Inter&outline_colour=ffffff&coffee_colour=FFDD00" /></a>



