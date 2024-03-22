#
# Copyright (C) 2016-2023 GitHub 
#
# This is free software, licensed under the GNU General Public License v3.
# See /LICENSE for more information.

include $(TOPDIR)/rules.mk

PKG_NAME:=s905d50
PKG_VERSION:=1.0
PKG_RELEASE:=68
PKG_LICENSE:=GPLv3
PKG_LICENSE_FILES:=LICENSE

include $(INCLUDE_DIR)/package.mk

define Package/s905d50
  SECTION:=luci
  CATEGORY:=LuCI
  TITLE:=LuCI support for LAN DHCP OFF Settings
  PKGARCH:=all
  DEPENDS:=+luci-base +luci-app-passwall +luci-app-ssr-plus
endef

define Package/s905d50/description
	Language Support Packages.
endef

define Build/Compile
endef

define Package/s905d50/install
	$(INSTALL_DIR) $(1)/etc/uci-defaults
	$(INSTALL_BIN) ./files/zzz-default-settings $(1)/etc/uci-defaults/99-s905d50
endef

$(eval $(call BuildPackage,s905d50))
