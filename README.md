<img src="https://i.imgur.com/CoKmZTU.png" width="500">

#### Requires Portal RTX for some DLLs.
1. Install Source SDK 2013 Multiplayer from Steam (search for it inside your library, it should show under Tools)
2. Download the latest version of [RTX Remix](https://github.com/NVIDIAGameWorks/rtx-remix/releases/download/remix-0.4.1/remix-0.4.1-release.zip), extract the archive into `steamapps\Source SDK Base 2013 Multiplayer\`
3. Download the Source SDK 2013 TF2 Port Client [here.](https://mega.nz/#!DZYhkIpC!oC9Pl_muYSPKLZGSRBubnI1kw4c9PNGbdXJCCi4qgfs) | (link from https://github.com/NicknineTheEagle/TF2-Base/releases/tag/v1.03)
4. Extract the `tf_port` folder from the archive to `steamapps\Source SDK Base 2013 Multiplayer\`
5. Download the patched [client](https://github.com/sambow23/TF2RTX-Stuff/raw/main/client.dll) and [engine](https://github.com/sambow23/TF2RTX-Stuff/raw/main/engine.dll) binaries from this repo
6. Move and replace the binaries at these locations
  - client.dll: `steamapps\Source SDK Base 2013 Multiplayer\tf_port\bin\client.dll`
  - engine.dll: `steamapps\Source SDK Base 2013 Multiplayer\bin\engine.dll`
7. Download [remix.bat](https://github.com/sambow23/TF2RTX-Stuff/raw/main/remix.bat) , [dxvk.conf](https://github.com/sambow23/TF2RTX-Stuff/raw/main/dxvk.conf) , and [rtx.conf](https://github.com/sambow23/TF2RTX-Stuff/raw/main/rtx.conf) from the repo and add it to `steamapps\Source SDK Base 2013 Multiplayer\`
8. grab `stdshader_dx6.dll, stdshader_dx7.dll, stdshader_dx8.dll, stdshader_dx9.dll` from `steamapps\PortalRTX\bin` and put them into `Source SDK Base 2013 Multiplayer\bin` replacing everything
9. Run the game with the `remix.bat`

#### Credits:
- [BlueAmulet for their Source Engine patches for RTX Remix](https://github.com/BlueAmulet/SourceRTXTweaks)
- @maksw2 on Discord
- @umfc on Discord
