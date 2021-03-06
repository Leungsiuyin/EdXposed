# EdXposed

A Riru module trying to provide a ART hooking framework (mainly for Android Pie) which delivers consistent APIs with the OG Xposed, leveraging YAHFA hooking framework.

## Credits 

- [YAHFA](https://github.com/rk700/YAHFA): the core java hooking framework
- [Riru](https://github.com/RikkaApps/Riru): provides a way to inject codes into zygote process
- [XposedBridge](https://github.com/rovo89/XposedBridge): the OG xposed framework APIs
- [dexmaker](https://github.com/linkedin/dexmaker) and [dalvikdx](https://github.com/JakeWharton/dalvik-dx): dynamiclly generate YAHFA hooker classes

## Known issues

- resources hooking is not supported yet
- may not be compatible with all ART devices
- only a few Xposed modules has been tested for working
- file access services are not implemented yet, now simply use magiskpolicy to enable needed SELinux policies

## Build

1. run `:Bridge:makeAndCopyRelease` in Gradle window to build `edxposed.dex`
2. run `:Core:zipRelease` to build Magisk Riru module flashable zip file
3. find the flashable under `Core/release/`
4. flash the zip in recovery mode or in Magisk Manager

## Install

1. make sure Magisk v17.0 or higher is installed.
2. download [Riru-core](https://github.com/RikkaApps/Riru/releases) v10 or higher and install it in Magisk Manager or recovery.
3. download [EdXposed](https://github.com/solohsu/EdXposed/releases) and install it in Magisk Manager or recovery.
4. reboot.
5. have fun :)

## Get help

GitHub issues(recommend): [Issues](https://github.com/solohsu/EdXposed/issues/)

QQ Group: [855219808](http://shang.qq.com/wpa/qunwpa?idkey=fae42a3dba9dc758caf63e971be2564e67bf7edd751a2ff1c750478b0ad1ca3f)

Telegream: [Code_of_MeowCat](http://t.me/Code_of_MeowCat)

Discord: [Code_of_MeowCat](https://discord.gg/Hag6gNh)

## Contribute

Apparently this framework is far from stable and all kinds of PRs are welcome. :)

