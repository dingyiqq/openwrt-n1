# Copyright (C) 2018 DingYi <dingyi139@gmail.com>
#
# This is free software, licensed under the Apache License, Version 2.0 .
#

include $(TOPDIR)/rules.mk

PKG_NAME:=s905d31
PKG_VERSION:=1.0
PKG_RELEASE:=68
PKG_LICENSE:=GPLv3
PKG_LICENSE_FILES:=LICENSE

PKG_BUILD_DIR := $(BUILD_DIR)/$(PKG_NAME)

include $(INCLUDE_DIR)/package.mk

define Package/s905d31
  SECTION:=luci
  CATEGORY:=LuCI
  TITLE:=LuCI support for LAN DHCP ON Settings
  PKGARCH:=all
  DEPENDS:=+luci-base +luci-app-passwall +luci-app-ssr-plus
endef

define Package/s905d31/description
	Language Support Packages.
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/s905d31/install
	$(INSTALL_DIR) $(1)/etc/uci-defaults
	$(INSTALL_BIN) ./files/zzz-default-settings $(1)/etc/uci-defaults/99-s905d31
endef

$(eval $(call BuildPackage,s905d31))
