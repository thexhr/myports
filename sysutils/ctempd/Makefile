COMMENT = color Temperature Changing Daemon

GH_ACCOUNT =	thexhr
GH_PROJECT =	ctempd
GH_TAGNAME =	2023.a

CATEGORIES =	sysutils

HOMEPAGE =	https://github.com/thexhr/ctempd

MAINTAINER =	Matthias Schmidt <openbsd@xosc.org>

# ISC
PERMIT_PACKAGE = Yes

# Uses pledge()
WANTLIB += c m X11 Xrandr

#LIB_DEPENDS =	devel/json-c \
#		security/libsodium

NO_TEST	=	Yes

.include <bsd.port.mk>
