<img src="https://i.imgur.com/CoKmZTU.png" width="500">

#### Requires [Portal RTX](https://store.steampowered.com/app/2012840/Portal_with_RTX/) for some DLLs.
1. Install Source SDK 2013 Multiplayer from Steam (search for it inside your library, it should show under Tools)
2. Download the latest version of [RTX Remix](https://github.com/NVIDIAGameWorks/rtx-remix/releases/download/remix-0.4.1/remix-0.4.1-release.zip), extract the archive into `steamapps\Source SDK Base 2013 Multiplayer\`
3. Download the Source SDK 2013 TF2 Port Client [here.](https://mega.nz/#!DZYhkIpC!oC9Pl_muYSPKLZGSRBubnI1kw4c9PNGbdXJCCi4qgfs) | (link from https://github.com/NicknineTheEagle/TF2-Base/releases/tag/v1.03)
4. Extract the `tf_port` folder from the archive to `steamapps\Source SDK Base 2013 Multiplayer\`
5. Download the patches [client](https://github.com/sambow23/TF2RTX-Stuff/raw/main/client.bps) and [engine](https://github.com/sambow23/TF2RTX-Stuff/raw/main/engine.bps) binaries from this repo
6. Download [Floating IPS](https://www.romhacking.net/utilities/1040/), extract it, open `flips.exe`, select `Apply Patch`
7. Select the .bps patch and then select the matching dll to patch in the locations below, then select it again, it should say: `The patch was applied successfully`.
  - client.dll: `steamapps\Source SDK Base 2013 Multiplayer\tf_port\bin\client.dll`
  - engine.dll: `steamapps\Source SDK Base 2013 Multiplayer\bin\engine.dll`
8. Download [remix.bat](https://github.com/sambow23/TF2RTX-Stuff/raw/main/remix.bat) , [dxvk.conf](https://github.com/sambow23/TF2RTX-Stuff/raw/main/dxvk.conf) , and [rtx.conf](https://github.com/sambow23/TF2RTX-Stuff/raw/main/rtx.conf) from the repo and add it to `steamapps\Source SDK Base 2013 Multiplayer\`
9. Grab `stdshader_dx6.dll, stdshader_dx7.dll, stdshader_dx8.dll, stdshader_dx9.dll` from `steamapps\PortalRTX\bin` and put them into `Source SDK Base 2013 Multiplayer\bin` replacing everything.
10. Run the game with the `remix.bat`, If you want to play with muliplayer, follow the guide below.

### Multiplayer
#### While this project isn't completely ready for multiplayer, it does work
#### DISCLAIMER: Please note that large maps like Hydro have poor performance because of the lack of culling
1. Copy the `tf_port` folder to the `%programfiles(x86)%\Steam\steamapps\sourcemods` folder **where _Steam_ is installed**, it won't work otherwise! After that restart Steam.
2. In Steam go to `Team Fortress 2 1.0.1.8 Port`, right click it and click `Properties`
3. In `Launch Options`, paste this line below into the field (change `-w` and `-h` to the resolution of your display, **do not change it ingame**)
- ```-dxlevel 70 -novid -w 1280 -h 720 -noborder -windowed +r_3dsky 0 +r_WaterDrawReflection 0 +r_WaterDrawRefraction 0 +r_shadows 0 +r_frustumcullworld 0 +r_unloadlightmaps 1 1 +mat_specular 0 +mat_bumpmap 0 +mat_normalmap 0 +mat_parallaxmap 0 +r_staticprop_lod 0```



#### Credits:
- [BlueAmulet for their Source Engine patches for RTX Remix](https://github.com/BlueAmulet/SourceRTXTweaks)
- @maksw2 on Discord
- @umfc on Discord
