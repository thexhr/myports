# $OpenBSD$

COMMENT =	player toolkit for the Ironsworn tabletop RPG

GH_ACCOUNT =	thexhr
GH_PROJECT =	isscrolls
GH_TAGNAME =	2022.c

CATEGORIES =	games

HOMEPAGE =	https://github.com/thexhr/isscrolls

MAINTAINER =	Matthias Schmidt <openbsd@xosc.org>

# ISC
PERMIT_PACKAGE = Yes

# Uses pledge()
WANTLIB += c json-c

LIB_DEPENDS =	devel/json-c

NO_TEST	=	Yes

.include <bsd.port.mk>
