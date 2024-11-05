#
# Copyright (C) 2024 allankevinrichie
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-asciidoc
PKG_VERSION:=10.2.1
PKG_RELEASE:=1

PYPI_NAME:=asciidoc
PKG_HASH:=d9f13c285981b3c7eb660d02ca0a2779981e88d48105de81bb40445e60dddb83

PKG_MAINTAINER:=allankevinrichie <allankevinrichie@outlook.com>
PKG_LICENSE:=GPLv2+
PKG_LICENSE_FILES:=LICENSE

PKG_BUILD_DEPENDS:=python3

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-asciidoc
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=AsciiDoc is a text document format for writing things
  URL:=https://github.com/asciidoc/asciidoc-py3
  DEPENDS:=+python3-light
endef

define Package/python3-asciidoc/description
AsciiDoc is a text document format for writing notes, documentation, articles, books, ebooks, slideshows, web pages, man pages and blogs. AsciiDoc files can be translated to many formats including HTML, PDF, EPUB, man page.

AsciiDoc.py is a legacy processor for this syntax, handling an older rendition of AsciiDoc. As such, this will not properly handle the current AsciiDoc specification. It is suggested that unless you specifically require the AsciiDoc.py toolchain, you should find a processor that handles the modern AsciiDoc syntax.

AsciiDoc.py is highly configurable: both the AsciiDoc source file syntax and the backend output markups (which can be almost any type of SGML/XML markup) can be customized and extended by the user.
endef

$(eval $(call Py3Package,python3-asciidoc))
$(eval $(call BuildPackage,python3-asciidoc))
$(eval $(call BuildPackage,python3-asciidoc-src))
