# Wineskin
Wineskin is a user-friendly tool used to make ports of Microsoft Windows software to macOS.\
Unlike the original [Wineskin Project](http://wineskin.urgesoftware.com) by doh123 that worked on *OS X 10.6* to *macOS 10.12* (without tweaks), this project supports *macOS 10.15* to *macOS 13*

<br>

## Want to help support this project?
[![ko-fi](https://img.shields.io/badge/kofi-Donate-blue?style=for-the-badge&logo=ko-fi)](https://ko-fi.com/gcenx)
[![PayPal](https://img.shields.io/badge/PayPal-Donate-blue?style=for-the-badge&logo=paypal)](https://www.paypal.com/paypalme/gcenx)

<br>

## How to install
### [homebrew](https://brew.sh/)
```
brew install --cask --no-quarantine gcenx/wine/wineskin
```

### Manual installation - (_not recommended!_)  
[Download Wineskin Winery](https://github.com/Gcenx/WineskinServer/releases/download/V1.8.4.2/Wineskin.Winery.txz)\
*_After downloading remove the flag quarantine before extraction, don't extract using __Keka___
```
/usr/bin/xattr -drs com.apple.quarantine Wineskin.Winery.txz
```

<br>

## DirectX support

__D3DMetal__\
Supports 64Bit DirectX 11 & 12 via Metal.\
Since "Game porting toolkit" 1.0 beta 4 Apple now allows redistriution for none commercial uses.\
You can view Apples documentionion [here](https://github.com/Gcenx/WineskinServer/tree/master/D3DMetal)

__WineD3D__\
Supports DirectX 11 and below.
- OpenGL backend is used for DirectX 9 and below
- Vulkan backend is used for DirectX 10 & 11
_Not useable in D3DMetal Engines_

__DXVK__\
Supports DirectX 10 & 11 via Vulkan.\
_DXVK is not compatible with D3DMetal Engines_

__VKD3D__\
Is currently not supported

<br>

## Hackintosh Support?
__AMD__ based systems are not supported due to being unable to run 32Bit code on macOS.  
__Intel__ based systems should work without issue.

<br>

# FAQ
### My Antivirus says it's a VIRUS!!!
You need to contact your Antivirus/Anti-malware vendor to report these as false positives.\
This started once wine moved to using *Mingw-gcc* to compile PE binaries.

__See the following examples:__
- [CrossOver 19 and antivirus programs](https://www.codeweavers.com/support/forums/general/?t=27;msg=222870)
- [Windows Defender detects Occamy.c trojan in steam proton 5.0 folder](https://github.com/ValveSoftware/Proton/issues/3593)

<br>

## License
Keeping the same as the original material, LGPL 2.1 is the license of that project. You can find more details about that in the LICENSE file.

<br>

## Credits
- [VitorMM](https://github.com/vitor251093) for modernizing the [Wineskin Codebase](https://github.com/vitor251093/wineskin) & [ObjectiveC_Extension](https://github.com/vitor251093/ObjectiveC_Extension).
- [PaulTheTall](https://www.paulthetall.com/) for constant test data and finding bugs.
- doh123 for creating [Wineskin](http://wineskin.urgesoftware.com).
- [thmrtz](https://github.com/thmrtnz) for the issue template, documentation and the wiki.
