#
# Copyright (C) 2018 DingYi <dingyi139@gmail.com>
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#
include $(TOPDIR)/rules.mk

BOARD:=armvirt
BOARDNAME:=QEMU ARM Virtual Machine
FEATURES:=fpu pci rtc usb
FEATURES+=cpiogz ext4 ramdisk squashfs targz
MAINTAINER:=DingYi <dingyi139@gmail.com>

KERNEL_PATCHVER:=4.14

include $(INCLUDE_DIR)/target.mk

DEFAULT_PACKAGES += bash blkid fdisk lsblk parted \
btrfs-progs kmod-fs-btrfs dosfstools e2fsprogs ntfs-3g \
gawk getopt losetup tar uuidgen

$(eval $(call BuildTarget))
