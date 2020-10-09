# Vupine

Minimalistic kernel edited for personal use, I do not advise using it.

## Why

Because I am stoopid.

### System

AMD FX-6300 oc'd to 4.20GHz, Radeon GIGABYTE RX 370 Windforce OC edition

### Building & Installing the kernel
1. Generate the .config `make vulpine_defconfig`
2. Build the kernel `make -j6`
3. Install the modules `make modules_install`
4. Copy the kernel to /boot dir `cp -v arch/x86/boot/bzImage /boot/vmlinuz-vulpine
5. Generate the initramfs images for the custom kernel `mkinitcpio -p vulpine
6. Reboot and hope for the best

## Authors

* **SnoopTheDog** - *Initial work* - [snoopie](https://github.com/SnoopTheDog)

## License
As stated at `https://github.com/torvalds/linux/blob/master/COPYING`:

The Linux Kernel is provided under:

	`SPDX-License-Identifier: GPL-2.0 WITH Linux-syscall-note`

Being under the terms of the GNU General Public License version 2 only,
according with:

	`LICENSES/preferred/GPL-2.0`

With an explicit syscall exception, as stated at:

	`LICENSES/exceptions/Linux-syscall-note`

In addition, other licenses may also apply. Please see:

	`Documentation/process/license-rules.rst`

for more details.

All contributions to the Linux Kernel are subject to this COPYING file.

## Acknowledgments

* Linus Torvalds
* [slanavoda](https://github.com/slanavoda)
