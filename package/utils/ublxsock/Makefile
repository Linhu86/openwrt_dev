#
# Copyright (C) 2010-2015 Jo-Philipp Wich <jow@openwrt.org>
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=ublxsockserver

PKG_RELEASE:=1

PKG_USE_MIPS16:=0


include $(INCLUDE_DIR)/package.mk

define Package/ublxsockserver
  SECTION:=utils
  CATEGORY:=Utilities
  TITLE:=ublxsockserver
  MAINTAINER:=linhu
endef

define Package/ublxsockserver/description
 Px5g is a tiny standalone X.509 certificate generator.
 It suitable to create key files and certificates in DER
 and PEM format for use with stunnel, uhttpd and others.
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Compile
	$(TARGET_CC) $(TARGET_CFLAGS) -o $(PKG_BUILD_DIR)/ublxsock server/ublxsockserver.c 
endef

define Package/ublxsockserver/install
	$(INSTALL_DIR) $(1)/usr/sbin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/ublxsock $(1)/usr/sbin/ublxsock
endef

$(eval $(call BuildPackage,ublxsockserver))
