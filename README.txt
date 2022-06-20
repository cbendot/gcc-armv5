armv5-eabi--glibc--bleeding-edge-2021.11-1

This is a toolchain provided by the https://toolchains.bootlin.com/
service. This toolchain was built using Buildroot.

The complete source code for all components of the toolchain can be
found at http://toolchains.bootlin.com/downloads/releases/sources/.

The complete license text of all components of the toolchain can be
found at http://toolchains.bootlin.com/downloads/releases/licenses/.

This toolchain is based on:

    gcc                  version     11.2.0
    binutils             version       2.37
    gdb                  version       11.1
    glibc                version 2.34-9-g9acab0bba6a5a57323b1f94bf95b21618a9e5aa4

For those who would like to reproduce the toolchain, you can just
follow these steps:

    git clone https://github.com/bootlin/buildroot-toolchains.git buildroot
    cd buildroot
    git checkout toolchains.bootlin.com-2021.11-1

    curl http://toolchains.bootlin.com/downloads/releases/toolchains/armv5-eabi/build_fragments/armv5-eabi--glibc--bleeding-edge-2021.11-1.defconfig > .config
    make olddefconfig
    make
    make sdk
