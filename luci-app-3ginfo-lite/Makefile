# Copyright 2021-2022 Rafał Wabik - IceG - From eko.one.pl forum
# MIT License

include $(TOPDIR)/rules.mk

PKG_NAME:=luci-app-3ginfo-lite
LUCI_TITLE:=LuCI panel for 3ginfo-lite
LUCI_PKGARCH:=all
LUCI_DEPENDS:=+sms-tool
PKG_VERSION:=1.0.20-20220809
PKG_RELEASE:=1

define Package/$(PKG_NAME)
	$(call Package/luci/webtemplate)
	TITLE:=$(LUCI_TITLE)
	DEPENDS:=$(LUCI_DEPENDS)
endef

define Package/$(PKG_NAME)/description
	LuCI panel for 3ginfo-lite.
endef

include $(TOPDIR)/feeds/luci/luci.mk

$(eval $(call BuildPackage,$(PKG_NAME)))

# call BuildPackage - OpenWrt buildroot signature
