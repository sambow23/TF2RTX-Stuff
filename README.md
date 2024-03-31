<img src="https://i.imgur.com/CoKmZTU.png" width="500">
<details><summary>Modern TF2</summary>

#### Multiplayer does not work VAC servers, do not try to curciumvent VAC protections for online play, use a patched or insecure server instead
1. Download the latest version of [RTX Remix](https://github.com/NVIDIAGameWorks/rtx-remix/releases/download/remix-0.4.1/remix-0.4.1-release.zip), extract the archive into `steamapps\Team Fortress 2\`
2. Download [BlueAmulet's SourceRTXTweaks Patcher](https://github.com/BlueAmulet/SourceRTXTweaks/raw/main/applypatch.py)
   - Right click the page and click `Save as...` and save it to `steamapps\Team Fortress 2\`
3. Download [remix.bat](https://github.com/sambow23/TF2RTX-Stuff/raw/main/tf2_modern/remix.bat) , [dxvk.conf](https://github.com/sambow23/TF2RTX-Stuff/raw/main/tf2_modern/dxvk.conf) , and [rtx.conf](https://github.com/sambow23/TF2RTX-Stuff/raw/main/tf2_modern/rtx.conf) from the repo and place them in `steamapps\Team Fortress 2\`
4. Install [Python](https://www.python.org/ftp/python/3.12.2/python-3.12.2-amd64.exe), make sure to click this option in the installer
   - <img src="https://i.imgur.com/oy7l4dl.png" width="250">
5. Open a CMD window inside of `steamapps\Team Fortress 2\`, run this command: `python applypatch.py`, the patched files will be located at `steamapps\Team Fortress 2\patched`.
6. Copy the two folders inside the patched folder and paste them in `steamapps\Team Fortress 2\`, overwriting everything
7. Run the game with the `remix.bat` file (if you want to change resolutions, open the file and change `-w` and `-h` to the resolution of your display, **do not change it ingame**).
8. For the game to not crash on map load, Open `Find a Game > Training > Offline Practice > King of The Hill > Nucleus > Start Practice`
9. After the map loads, you can load almost any map with the console
 </details>

<details><summary>TF2 2008 SDK 2013 Port</summary>
  
#### Requires [Portal RTX](https://store.steampowered.com/app/2012840/Portal_with_RTX/) for some DLLs.
1. Install Source SDK 2013 Multiplayer from Steam (search for it inside your library, it should show under Tools).
2. Download the latest version of [RTX Remix](https://github.com/NVIDIAGameWorks/rtx-remix/releases/download/remix-0.4.1/remix-0.4.1-release.zip), extract the archive into `steamapps\Source SDK Base 2013 Multiplayer\`
3. Download the Source SDK 2013 TF2 Port Client [here.](https://mega.nz/#!DZYhkIpC!oC9Pl_muYSPKLZGSRBubnI1kw4c9PNGbdXJCCi4qgfs) | (link from https://github.com/NicknineTheEagle/TF2-Base/releases/tag/v1.03).
4. Extract the `tf_port` folder from the archive to `steamapps\Source SDK Base 2013 Multiplayer\`
5. Download the patches [client](https://github.com/sambow23/TF2RTX-Stuff/raw/main/client.bps) and [engine](https://github.com/sambow23/TF2RTX-Stuff/raw/main/engine.bps) binaries from this repo.
6. Download [Floating IPS](https://www.romhacking.net/utilities/1040/), extract it, open `flips.exe`, select `Apply Patch`.
7. Select the .bps patch and then select the matching dll to patch in the locations below, then select it again, it should say: `The patch was applied successfully`.
  - client.dll: `steamapps\Source SDK Base 2013 Multiplayer\tf_port\bin\client.dll`
  - engine.dll: `steamapps\Source SDK Base 2013 Multiplayer\bin\engine.dll`
8. Download [remix.bat](https://github.com/sambow23/TF2RTX-Stuff/raw/main/tf2_port/remix.bat) , [dxvk.conf](https://github.com/sambow23/TF2RTX-Stuff/raw/main/tf2_port/dxvk.conf) , and [rtx.conf](https://github.com/sambow23/TF2RTX-Stuff/raw/main/tf2_port/rtx.conf) from the repo and add it to `steamapps\Source SDK Base 2013 Multiplayer\`
9. Grab `stdshader_dx6.dll, stdshader_dx7.dll, stdshader_dx8.dll, stdshader_dx9.dll` from `steamapps\PortalRTX\bin` and put them into `Source SDK Base 2013 Multiplayer\bin` replacing everything.
10. Run the game with the `remix.bat`, If you want to play with muliplayer, follow the guide below.

### Multiplayer
#### While this project isn't completely ready for multiplayer, it does work.
#### DISCLAIMER: Please note that large maps like Hydro have poor performance because of the lack of culling.
1. Copy the `tf_port` folder to the `%programfiles(x86)%\Steam\steamapps\sourcemods` folder **where _Steam_ is installed**, it won't work otherwise! After that restart Steam.
2. In Steam go to `Team Fortress 2 1.0.1.8 Port`, right click it and click `Properties`.
3. In `Launch Options`, paste this line below into the field (change `-w` and `-h` to the resolution of your display, **do not change it ingame**).
- ```-dxlevel 70 -novid -w 1280 -h 720 -noborder -windowed +r_3dsky 0 +r_WaterDrawReflection 0 +r_WaterDrawRefraction 0 +r_shadows 0 +r_frustumcullworld 0 +r_unloadlightmaps 1 1 +mat_specular 0 +mat_bumpmap 0 +mat_normalmap 0 +mat_parallaxmap 0 +r_staticprop_lod 0```

 </details>


#### Credits:
- [BlueAmulet for their Source Engine patches for RTX Remix](https://github.com/BlueAmulet/SourceRTXTweaks)
- @maksw2 on Discord
- @umfc on Discord
- @popo7235 on Discord
