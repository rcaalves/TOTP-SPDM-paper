# TOTP-SPDM-buildroot-module (WIP)
Buildroot module for TOTP + SPDM integration

This project uses [libpsdm](https://github.com/DMTF/libspdm/), which must be built separately on the host machine.

Instructions:
- Integrating libpsdm to qemu and the kernel is explained at https://github.com/rcaalves/spdm-hd-demo
- Copy the files in the [drivers](drivers) directory into the kernel tree (`output/build/linux-[version.number]` in Buildroot)
- Recompile the kernel. Set `SPDM_DIR` and `SPDM_BUILD_DIR` variables properly
	- E.g. `make SPDM_DIR=path/to/libspdm SPDM_BUILD_DIR=path/to/libspdm/build_buildroot linux-rebuild`
