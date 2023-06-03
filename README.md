# NoTouchID
Lilu plugin for disabling Touch ID support.

Modified the project to be build with MacKernelSDK
#

###
original project and Credits to [al3xtjames]( https://github.com/al3xtjames/NoTouchID)
#
### To build
git clone [Lilu](https://github.com/acidenthera/Lilu)
build as debug

then

git clone [NoTouchID](https://github.com/AcoUk/NoTouchID)

cd NoTouchID && git clone [MacKernelSDK](https://github.com/acidenthera/MacKernelSDK)

build for your target machine
#
BiometricKit.framework in 10.13.4+ assumes a Touch ID sensor is present when a compatible board ID is used, which causes lag in authentication dialogs (as well as a delayed login screen). Patching this out resolves such hangs.

This issue appears to have been fixed on 10.15.7 and 11.0.1. This kext is unnecessary on these versions of macOS.
Configuration

    Add -nobiooff to disable NoTouchID
    Add -nobiobeta to enable NoTouchID on unsupported OS versions (10.13-10.15 are supported by default)

Downloads

Available on the releases page.
