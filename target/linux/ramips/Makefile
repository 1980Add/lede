#
# Copyright (C) 2008-2011 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#
include $(TOPDIR)/rules.mk

ARCH:=mipsel
BOARD:=ramips
BOARDNAME:=MediaTek Ralink MIPS
SUBTARGETS:=mt7620 mt7621 mt76x8 rt288x rt305x rt3883
FEATURES:=squashfs gpio

KERNEL_PATCHVER:=4.14
KERNEL_TESTING_PATCHVER:=4.14

define Target/Description
	Build firmware images for Ralink RT288x/RT3xxx based boards.
endef

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += kmod-leds-gpio kmod-gpio-button-hotplug -luci-app-sfe luci-app-flowoffload

$(eval $(call BuildTarget))
