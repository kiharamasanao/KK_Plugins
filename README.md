Support me on Patreon!<br/>
https://www.patreon.com/DeathWeasel

# KK_Plugins
Plugins for Koikatsu, EmotionCreators, and AI Girl

## Installation
1. Install [BepInEx v5.0](https://github.com/BepInEx/BepInEx/releases)
2. Install [BepisPlugins](https://github.com/bbepis/BepisPlugins/releases)
3. Install [IllusionModdingAPI](https://github.com/IllusionMods/IllusionModdingAPI)
4. Extract the plugin .zip file to your game folder

#### CharaMakerLoadedSound
**v1.0 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v1/KK_CharaMakerLoadedSound.v1.0.zip)** - For Koikatsu<br/>

Plays a sound when the Chara Maker finishes loading. Useful if you spend the load time alt-tabbed.

#### StudioSceneLoadedSound
**v1.1 - [Download](https://www.patreon.com/posts/32459105)** - For Koikatsu and AI Girl<br/>

Plays a sound when a Studio scene finishes loading or importing. Useful if you spend the load time for large scenes alt-tabbed.<br/>

<details><summary>Change Log</summary>
v1.1 Config options, AI version (thanks GeBo!)<br/>
</details>

#### ForceHighPoly
**v1.2 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v70/KK_ForceHighPoly.v1.2.zip)** - For Koikatsu<br/>

Forces all characters to load in high poly mode, even in the school exploration mode.<br/>

<details><summary>Change Log</summary>
v1.1 Fixed locking up the game after special H scenes. Added config option to disable high poly mode.<br/>
v1.2 Fixed hair physics not working (Thanks Rau/Marco/Essu)<br/>
</details>

#### ReloadCharaListOnChange
**v1.5.1 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v91/KK_ReloadCharaListOnChange.v1.5.1.zip)** - For Koikatsu<br/>

Reloads the list of characters and coordinates in the character maker when any card is added or removed from the folders. Supports adding and removing large numbers of cards at once.<br/>

<details><summary>Change Log</summary>
v1.1 Fixed new coordinates saved from within the game not being handled correctly<br/>
v1.2 Fixed error when exiting the chara maker<br/>
v1.3 Updated for plugin compatibility<br/>
v1.4 Studio support<br/>
v1.4.1 Compatibility with BepisPlugins versions higher than r8<br/>
v1.5 Koikatsu Party compatibility<br/>
v1.5.1 Create card folders if missing to prevent errors<br/>
</details>

#### InvisibleBody
**v1.3.2 - [Download](https://www.patreon.com/posts/28424780)** - For Koikatsu, Emotion Creators, and AI Girl<br/>

Set the Invisible Body toggle for a character in the character maker to hide the body. Any worn clothes or accessories will remain visible.<br/>

Select characters in the Studio workspace and Anim->Current State->Invisible Body to toggle them between invisible and visible. Any worn clothes or accessories and any attached studio items will remain visible. Invisible state saves and loads with the scene. <br/>

<details><summary>Change Log</summary> 
v1.1 Fixed studio items becoming visible when they were toggled off in the workspace<br/>
v1.2 Added a character maker toggle, EmotionCreators port<br/>
v1.2.1 Fixed an incompatibility with UncensorSelector<br/>
v1.2.2 Updated for KK Darkness<br/>
v1.3 Added a toggle button for Studio, removed hotkey<br/>
v1.3.1 Fixed accessories and items attached by animations from turning invisible in AI version<br/>
v1.3.2 Fixed Studio items turning invisible in AI version<br/>
</details>

#### InputHotkeyBlock
**v1.2 - [Download](https://www.patreon.com/posts/29761547)** - For Koikatsu and AI Girl<br/>

Blocks mod hotkeys from triggering while typing in input fields and prevents clicks inside mod GUIs from advancing the story.

Credits:
* essu: Code for blocking hotkeys
* Kyne: Code for preventing mod GUI clicks from advancing the story in Koikatsu

<details><summary>Change Log</summary>
v1.1 Blocks hotkeys in studio coordinate fields<br/>
v1.2 Prevents clicks inside mod GUI elements from advancing the story in Koikatsu (Thanks Kyne)<br/>
</details>

#### UncensorSelector
**v3.9 - [Download](https://www.patreon.com/posts/28204946)** - For Koikatsu, Emotion Creators, and AI Girl<br/>

Download uncensors:<br/>
For Koikatsu click [here.](https://mega.nz/#F!upYGBTAZ!S1lMalC33LYEditk7GwzgQ!S0IzlILZ)<br/>
For EmotionCreators click [here.](https://mega.nz/#F!upYGBTAZ!S1lMalC33LYEditk7GwzgQ!u4pUmKzb)<br/>

Allows you to specify which uncensors individual characters use and removes the mosaic censor. Select an uncensor for your character in the character maker in the Body/General tab or specify a default uncensor to use in the plugin settings. The default uncensor will apply to any character that does not have one selected.<br/>

Requirements:
* Marco's [KKAPI](https://github.com/ManlyMarco/KKAPI/releases)
* Marco's [Overlay Mods](https://github.com/ManlyMarco/Koikatu-Overlay-Mods/releases)
* [BepisPlugins](https://github.com/bbepis/BepisPlugins/releases) ExtensibleSaveFormat and Sideloader.

UncensorSelector compatible uncensors can be found [here.](https://mega.nz/#F!upYGBTAZ!S1lMalC33LYEditk7GwzgQ!n54h1KZS) For makers of uncensors, see the [template](https://github.com/DeathWeasel1337/KK_Plugins/blob/master/Core_UncensorSelector/Template.xml) for how to configure your uncensor for UncensorSelector compatibility.<br/>

Make sure to remove any sideloader uncensors and replace your oo_base with a clean, unmodified one to prevent incompatibilities!<br/>

<details><summary>Change Log</summary>
v2.0 Complete rewrite, now supports changing uncensors inside the character maker, configuring uncensor metadata in manifest.xml, demosaic, etc.<br/>
v2.1 Reduce reliance on KK_UncensorSelector Base.zipmod<br/>
v2.2 Removed the ability to specify _low assets. A matching _low asset is expected to exist for everything that requires one.<br/>
v2.3 Added some warning labels<br/>
v2.4 Fixed demosaic not working sometimes<br/>
v2.5 ConfigManager dropdown for GUID selection, fixed color matching bug in chara maker<br/>
v2.6 Uncensors now change much more quickly without causing lag in the character maker. Random can be selected as an option for the default uncensor, any character with no uncensor selected will use a random one (Thanks @ManlyMarco). Uncensors can be exluded from random selection with a modification to the manifest.xml.<br/>
v2.6.1 Fix for the new uncensor loading code breaking in low poly<br/>
v2.7 Names in ConfigManager instead of GUIDs, uncensor lists are ordered (Thanks @ManlyMarco), slightly faster uncensor switching<br/>
v3.0 All uncensors load correctly in the character maker, default uncensors display in character maker, body parts can be selected independently from the body, new format for uncensors, new bugs<br/>
v3.1 Fixed uncensors not loading in the character maker accessed through the class menu, fixed some low poly uncensors not display correctly for the main character, fixed low poly uncensors not working at all for female characters<br/>
v3.2 Random uncensors are now more evenly distributed, gender bender config option simplified, fixed a problem with clothes that have the same mesh name as body part meshes causing problems<br/>
v3.3 Fix wrong normals after loading a character sometimes, fix default values when loading a character in to the character maker from class menu, fix balls dropdown not reloading the uncensor on change<br/>
v3.4 Fix liquid textures being removed on changing characters<br/>
v3.5 Added a message that displays if the skin texture has become corrupt and attempts a fix (Thanks @ManlyMarco)<br/>
v3.5.1 Reduce false positives for the above change<br/>
v3.6 EmotionCreators port, removed "none" as a default config option<br/>
v3.6.1 Updated for KK Darkness<br/>
v3.6.2 Fix replacing janitor's body when it shouldn't<br/>
v3.6.3 Fix janitor's uncensor<br/>
v3.6.4 Fix compatibility issues for non Darkness game versions<br/>
v3.7 Fix shadows on male parts and reduce error spam<br/>
v3.8 AI Girl version<br/>
v3.8.1 Fix broken config stuff (thanks Keelhauled)<br/>
v3.8.3 Fix uncensors not working in AI Girl main game<br/>
v3.9 Fix crash with duplicate uncensor GUIDs, implement dick/balls support for AI Girl<br/>
v3.9.1 Fix error in Studio resulting from having no uncensors<br/>
</details>

#### Subtitles
**v1.4 - [Download](https://www.patreon.com/posts/27699376)** - For Koikatsu<br/>
**v1.5.1 - [Download](https://www.patreon.com/posts/27699376)** - For AI Girl<br/>

For Koikatsu, adds subtitles for H scenes, spoken text in dialogues, and character maker.<br/>
For AI Girl trial version, adds subtitles for the character maker.<br/>

<details><summary>Change Log</summary>
v1.1 Fixed H subs not working for some people<br/>
v1.2 Subtitles for idle lines in dialogue<br/>
v1.3 Subtitles for character maker<br/>
v1.4 Fixed subtitles in the character maker being under the UI<br/>
v1.5 AI Girl port<br/>
v1.5.1 Fixed text wrapping, clarified config description<br/>
</details>

#### AnimationController
**v2.2 - [Download](https://www.patreon.com/posts/31229780)** - For Koikatsu and AI Girl<br/>
*Koikatsu version: Mostly obsolete. [NodeConstraints](https://www.patreon.com/posts/26357789) does what this plugin does but better.*

Allows attaching IK nodes to objects to create custom animations. Press the Minus (-) hotkey to bring up the menu. This hotkey can be  configured in the F1 plugin settings.<br/>

Requires Marco's [KKAPI](https://github.com/ManlyMarco/KKAPI/releases) and [BepisPlugins](https://github.com/bbepis/BepisPlugins/releases) ExtensibleSaveFormat.<br/>

Inspired by [AttachAnimationLib](http://www.hongfire.com/forum/forum/hentai-lair/hf-modding-translation/honey-select-mods/6388508-vn-game-engine-ready-games-and-utils?p=6766050#post6766050) by Keitaro  

<details><summary>Change Log</summary>
v1.1 Gimmicks can now rotate hands and feet properly<br/>
v1.2 Rotating characters doesn't break everything anymore<br/>
v2.0 Significant rewrite with KKAPI integration. Can now link eyes and neck to objects, scene import support, Drag and Drop plugin support<br/>
v2.1 Fix neck link not working, fix linking after unlinking not working<br/>
v2.2 AI version, window position adjustment<br/>
</details>

#### ClothingUnlocker
**v1.1 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v62/KK_ClothingUnlocker.v1.1.zip)** - For Koikatsu<br/>
**v1.1 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v77/EC_ClothingUnlocker.v1.1.zip)** - For EmotionCreators<br/>

Allows gender restricted clothing to be used on all characters.<br/>

<details><summary>Advanced mode</summary>
KK_ClothingUnlocker can unlock bras/skirts with any top. Go to plugin settings and enable advanced mode to see the options for them. These settings are not recommended because they will require updating many characters for compatibility.<br/>
</details>

<details><summary>Change Log</summary>
v1.1 Added clothing unlocking for bras/skirts with any top<br/>
</details>

#### EyeShaking
**v1.0 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v38/KK_EyeShaking.v1.0.zip)** - For Koikatsu<br/>

Virgins in H scenes will appear to have slightly shaking eye highlights.<br/>

#### RandomCharacterGenerator
**v1.0 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v47/KK_RandomCharacterGenerator.v1.0.zip)** - For Koikatsu<br/>

Generates random characters in the character maker.<br/>

#### PoseFolders
**v1.0 - [Download](https://www.patreon.com/posts/31127973)** - For Koikatsu and AI Girl<br/>

Create new folders in userdata/studio/pose and place the pose data inside them. Folders will show up in your list of poses in Studio.<br/>

Ported from Essu's NEOpose List Folders plugin for Honey Select.<br/>

#### TranslationSync
**v1.2 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v61/KK_TranslationSync.v1.2.zip)** - For Koikatsu<br/>

A plugin for correctly formatting translation files. Corrects formatting and copies translations from one file to another for the same personality in case of duplicate entries. Used by translators working on the [Koikatsu Translation](https://github.com/DeathWeasel1337/Koikatsu-Translations) project. No need to download unless you're working on translations.<br/>

To use, open the plugin settings and set a personality, press the hotkey (default 0) to sync translations. Read your bepinex console or output_log.txt to see the changes made or any warnings and errors. Press alt+hotkey to force sync translation files in case of differing translations (warning: make backups first. It may not be obvious which translations are treated as the primary source). Press ctrl+hotkey to sync translations for all personalities (warning: very slow).<br/>

#### ListOverride
**v1.0 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v65/KK_ListOverride.v1.0.zip)** - For Koikatsu<br/>

Allows you to override vanilla list files. Comes with some overrides that enable half off state for some vanilla pantyhose.<br/>

Overriding list files can allow you to do things like enable bras with some shirts which don't normally allow it, or skirts with some tops, etc. Any part of of the list can be changed except for ID.<br/>

#### HairAccessoryCustomizer
**v1.1.3 - [Download](https://www.patreon.com/posts/27712341)** - For Koikatsu and Emotion Creators<br/>

Adds configuration options for hair accessories to the character maker. Hair accessories can be set to match color with the hair, enable hair gloss, modify outline color, and has a separate color picker for the hair tie part. Hairs that support a length slider can also hair their length adjusted, just like vanilla front hairs. Saves and loads to cards and coordinates.<br/>

Configuration options will work only on properly configured hair accessories. All of the hair accessories from <https://mega.nz/#F!upYGBTAZ!S1lMalC33LYEditk7GwzgQ!GpJEiLwK> will work.<br/>

Requires Marco's [KKAPI](https://github.com/ManlyMarco/KKAPI/releases) v1.3 or higher, previous versions will NOT work.<br/>

Note for modders: These options will only show up for hair accessories that are properly configured. For accessories to work the accessory must have a ChaCustomHairComponent MonoBehavior in addition to the ChaAccessoryComponent MonoBehavior. Hair accessory color will display if the ChaCustomHairComponent rendAccessory array has meshes configured. The length slider will appear if the ChaCustomHairComponent trfLength array has bones configured. Hair color will only match to meshes configured in the ChaCustomHairComponent rendHair array. Also check out [this guide](https://github.com/DeathWeasel1337/KK_Plugins/wiki/Hair-Accessory-Guide) for how to create hair accessories.<br/>

<details><summary>Change Log</summary>
v1.1 Fixed a bug with changing coordinates outside of Studio not applying color matching. Fixed a bug where changing hair color in the maker would not apply color matching to other outfit slots.<br/>
v1.1.1 Fixed hair accessories matching color when they shouldn't.<br/>
v1.1.2 Fixed hair accessories matching color when they shouldn't, again.<br/>
v1.1.3 Fixed an error when starting the classroom character maker.<br/>
</details>

#### Demosaic
**v1.1 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v73/EC_Demosaic.v1.1.zip)** - For EmotionCreators<br/>
Note: Not required when using UncensorSelector<br/>

Removes the mosaic from female characters. Based on the demosaic for Koikatsu by [AUTOMATIC1111](https://github.com/AUTOMATIC1111/KoikatsuMods), compiled for EC and BepInEx 5.<br/>

<details><summary>Change Log</summary>
v1.1 Added a config option to disable the plugin<br/>
</details>

#### FreeHRandom
**v1.1.1 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v91/KK_FreeHRandom.v1.1.1.zip)** - For Koikatsu<br/>
Adds buttons to Free H selection screen to get random characters for your H session.<br/>

<details><summary>Change Log</summary>
v1.1 Added UI, KK Party support<br/>
v1.1.1 Create card folders if missing to prevent errors<br/>
</details>

#### Colliders
**v1.0 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/download/v37/KK_Colliders.v1.0.zip)** - For Koikatsu<br/>

Adds floor, breast, hand, and skirt colliders. Ported from Patchwork.<br/>

#### MaterialEditor
**v1.9.1 - [Download](https://www.patreon.com/posts/27881027)** - For Koikatsu, EmotionCreators, and AI Girl<br/>
MaterialEditor is a plugin that allows you to edit many properties of objects that aren't usually accessible in game. Much like [Marco's clothing overlays](https://github.com/ManlyMarco/Koikatu-Overlay-Mods) you can replace the texture of an item, however with MaterialEditor you can edit much more than clothes. Edit clothes, accessories, hair, and even Studio items.

Features:
* Export UV maps of a mesh to help with drawing textures
* Replace nearly any texture with custom textures
* Change properties of materials to control things like shininess or outline thickness
* Change properties of the mesh to affect whether it casts shadows or disable a mesh completely
* Change the shader of a material
* All changes save and load with the card or Studio scene
* Duplicate textures are saved to the card once. 100 accessories with the same texture have the same file size as one accessory with a texture

Access the Material Editor by pressing the "Open Material Editor" button on clothes, hair, or accessories in the character maker. Access it in Studio by pressing the "Mat. Editor" button on the Workspace with a studio item selected.

<details><summary>Change Log</summary>
v1.1 Fixed errors loading coordinates, errors loading scenes with multiple characters<br/>
v1.2 Added the ability to change body and face materials<br/>
v1.3 Copied studio items now copy Material Editor settings, changed filename format<br/>
v1.3.1 Fixed error on importing studio objects with textures<br/>
v1.4 Add ability to change shaders, change skin and face material<br/>
v1.4.1 .jpg loading support, scroll speed increase, color and texture default values for custom shaders<br/>
v1.5 Added main_skin shader, removed alpha_a and alpha_b properties for character skin<br/>
v1.6 AI version<br/>
v1.7 Add sliders<br/>
v1.8 AI Studio support<br/>
v1.9 Fixed data lost on changing clothing color and copying accessories, add texture offset and scale, add indicator mark for changed properties, add support for MainTex replacement<br/>
v1.9.1 Fixed mipmaps not being generated, fixed error on object copy in Studio, added ability to resize the UI<br/>
</details>

#### MaleJuice
**v1.1 - [Download](https://www.patreon.com/posts/28608195)** - For Koikatsu<br/>

Enables juice textures for males in H scenes and Studio.<br/>

<details><summary>Change Log</summary>
v1.1 Fixed compatibility issues with UncensorSelector using male body type on female characters<br/>
</details>

#### StudioObjectMoveHotkeys
**v1.0 - [Download](https://www.patreon.com/posts/28743884)** - For Koikatsu and AI Girl<br/>

Allows you to move objects in studio using hotkeys. Press Y/U/I to move along the X/Y/Z axes. You can also use these keys for rotating and scaling, and when scaling you can also press T to scale all axes at once. Hotkeys can be configured in plugin settings.<br/>

#### FKIK
**v1.1 - [Download](https://www.patreon.com/posts/29928651)** - For Koikatsu and AI Girl<br/>

Enables FK and IK at the same time. Pose characters in IK mode while still being able to adjust skirts, hair, and hands as if they were in FK mode.<br/>

<details><summary>Change Log</summary>
v1.1 Fix toggles going out of sync, FK being disabled when switching between characters<br/>
</details>

#### AnimationOverdrive
**v1.1 - [Download](https://www.patreon.com/posts/31292617)** - For Koikatsu and AI Girl<br/>

Type in to the animation speed box in Studio for gimmicks and character animations to go past the normal limit of 3.<br/>

<details><summary>Change Log</summary>
v1.1 AI Girl port, capped animation speed at 1000 to prevent animations breaking<br/>
</details>

#### TextResourceRedirector
**v1.1 - [Download](https://github.com/DeathWeasel1337/KK_Plugins/releases/tag/v129)** - For Koikatsu, HoneySelect, and AI Girl<br/>

Allows translations to override individual assets. Required for some translations to function correctly. Requires [Unity.AutoTranslator](https://github.com/bbepis/XUnity.AutoTranslator).

#### CharacterExport
**v1.0 - [Download](https://www.patreon.com/posts/32434052)** - For Koikatsu, EmotionCreators, and AI Girl<br/>

Press Ctrl+E (configurable) to export all loaded character. Used for exporting characters from Studio scenes and such.<br/>

#### HCharaAdjustment
**v2.0 - [Download](https://www.patreon.com/posts/32552349)** - For Koikatsu<br/>
Adjust the position of the female character in H scene by pressing some hotkeys, which are configurable in the plugin settings.<br/>

<details><summary>Change Log</summary>
v1.0.1 Made the hotkeys configurable<br/>
v2.0 Added a guide object instead of hotkeys for positioning<br/>
</details>

#### KK_CutsceneLockupFix
#### KK_HeadFix
#### KK_MiscFixes
#### KK_PersonalityCorrector
#### KK_SettingsFix
Moved to the [IllusionFixes](https://github.com/IllusionMods/IllusionFixes) repo.<br/>

#### GUIDMigration
Obsolete, features merged in to Sideloader iself
