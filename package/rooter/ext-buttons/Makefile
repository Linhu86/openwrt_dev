#Owned by DairyMan@Whirlpool
#
#Copyright GNU act.
include $(TOPDIR)/rules.mk

PKG_NAME:=ext-buttons
PKG_VERSION:=1.000
PKG_RELEASE:=1

PKG_MAINTAINER:=Created by DM/makefile by Cobia@whirlpool
include $(INCLUDE_DIR)/package.mk

define Package/ext-buttons
  SECTION:=utils
  CATEGORY:=Network
  TITLE:=Install ext-buttons
  PKGARCH:=all
endef

define Package/ext-buttons/description
  Helper scripts to install ext-buttons
endef


define Build/Compile
endef

define Package/ext-buttons/install
	$(CP) ./files/* $(1)/


endef

$(eval $(call BuildPackage,ext-buttons))
