# Eclipse + OpenOCD + ARM GCC + CMSIS Pack Manager PlugIn

----

## 環境安裝

下載安裝Eclipse IDE for Embedded C/C++ Developers

https://www.eclipse.org/downloads/packages/release/2021-12/r/eclipse-ide-embedded-cc-developers

安裝至D:\Users\username\eclipse    

![](image/2022-03-03-10-59-39-image.png)

更新Eclipse Embedded CDT plug-ins v6.1.2    
[https://eclipse-embed-cdt.github.io/blog/2021/03/05/plugins-v6.1.2-released](https://eclipse-embed-cdt.github.io/blog/2021/03/05/plugins-v6.1.2-released/)

Instell New Software加入Embedded CDT plug-ins weblink     
https://download.eclipse.org/embed-cdt/releases/6.1.2/p2/

![](image/2022-03-02-14-05-06-image.png)

更新Embedded CDT plug-ins

![](image/2022-03-02-15-03-01-image.png)

新增CMSIS-Pack Manager PlugIn, 下載zip至D:\Users\username\eclipse\demo\ARM-software

https://github.com/ARM-software/cmsis-pack-eclipse/releases/tag/v2.6.1

Instell New Software加入CMSIS-Pack Manager Plug (D:\Users\username\eclipse\demo\ARM-software\CmsisPackPlugIn2.6.1.zip)

![](image/2022-03-02-16-40-48-image.png)

GUI加入CMSIS-Pack Manager

<img title="" src="image/2022-03-03-09-30-06-image.png" alt="" data-align="inline">

![](image/2022-03-03-09-30-49-image.png)

下載ARM CMSIS 5.8.0, CMSIS-Pack Manager將檔案存放在C:/Users/username/AppData/Local/Arm/Packs

![](image/2022-03-03-09-37-28-image.png)

下載xpack-dev-tools arm-none-eabi-gcc,openocd,windows-build-tools, 解壓縮至D:\Users\username\eclipse\demo\xPack

[https://github.com/xpack-dev-tools/arm-none-eabi-gcc-xpack/releases/tag/v10.3.1-2.3](https://github.com/xpack-dev-tools/arm-none-eabi-gcc-xpack/releases/tag/v10.3.1-2.3)

[https://github.com/xpack-dev-tools/openocd-xpack/releases/tag/v0.11.0-3](https://github.com/xpack-dev-tools/openocd-xpack/releases/tag/v0.11.0-3)

[https://github.com/xpack-dev-tools/windows-build-tools-xpack/releases/tag/v4.2.1-2](https://github.com/xpack-dev-tools/windows-build-tools-xpack/releases/tag/v4.2.1-2)

![](image/2022-03-02-16-36-40-image.png)

設定MCU Global Arm Toolchans Paths, D:\Users\username\eclipse\demo\xPack\xpack-arm-none-eabi-gcc-10.3.1-2.3\bin

![](image/2022-03-02-16-37-11-image.png)

設定MCU Global Build Tools Paths, D:\Users\username\eclipse\demo\xPack\xpack-windows-build-tools-4.2.1-2\bin

![](image/2022-03-02-16-37-26-image.png)

設定MCU Global OpenOCD Path, D:\Users\username\eclipse\demo\xPack\xpack-openocd-0.11.0-3\bin

![](image/2022-03-02-16-37-41-image.png)

設定CMSIS-Packs目錄, C:/Users/username/AppData/Local/Arm/Packs

![](image/2022-03-03-09-41-39-image.png)

---

## 新增CMSIS專案

新增C/C++ Project專案

![](image/2022-03-02-16-00-40-image.png)

選擇C Managed Build

![](image/2022-03-02-16-02-14-image.png)

選擇CMSIS C/C++ Project type, ToolChains選擇Arm Cross GCC

![](image/2022-03-02-16-02-46-image.png)

Device選擇ARMCM55

![](image/2022-03-02-16-03-32-image.png)

![](image/2022-03-02-16-03-51-image.png)

![](image/2022-03-02-16-04-08-image.png)

![](image/2022-03-02-16-04-23-image.png)

加入main.c

```
#include <stdio.h>

int
main(void)
{
  printf("Hello Arm World!" "\n");
  return 0;
}
```

開啟myCMSIS_cortexM55.rteconfig , 勾選CMSIS Core和Device Startup, Ctrl + S 自動複製到myCMSIS_cortexM55專案的RTE

![](image/2022-03-02-16-06-38-image.png)

修改專案Properties

![](image/2022-03-02-16-10-35-image.png)

將Arm famly cortex-m3改為cortex-m33

![](image/2022-03-02-16-11-09-image.png)

勾選"Do not use syscalls"

![](image/2022-03-02-16-12-08-image.png)

Build Project

![](image/2022-03-02-16-14-24-image.png)

編譯通過

![](image/2022-03-02-16-14-42-image.png)

使用Zadig對FT232H (VID 0403, PID 0614)使用winUSB取代

https://zadig.akeo.ie/

![](image/2022-03-02-16-30-31-image.png)

![](image/2022-03-02-16-32-09-image.png)

由於Windows inbox driver 支援FTDI Serial裝置 , Windows將FT232H視定為COM and LPT裝置

![](image/2022-03-02-16-33-16-image.png)

![](image/2022-03-02-16-33-42-image.png)

winUSB取代後, Windows將FT232H視為通用序列匯流排裝置

![](image/2022-03-02-16-32-30-image.png)

設定Debug Configurations

![](image/2022-03-02-16-15-46-image.png)

Debugger Config options加入openocd command

![](image/2022-03-02-16-17-54-image.png)

D:\Users\username\eclipse\demo\xPack\xpack-openocd-0.11.0-3\bin\ft232h-swd.cfg

```
source [find interface/ftdi/ft232h-module-swd.cfg]
source [find target/stellaris.cfg]
```

按Debug,可以看到openocd 認到FT232H, 但FT232H沒接裝置

![](image/2022-03-02-16-28-21-image.png)

![](image/2022-03-02-21-13-05-image.png)
