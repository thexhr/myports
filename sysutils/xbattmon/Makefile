# $OpenBSD: Makefile,v 1.1.1.1 2017/11/13 17:24:12 steven Exp $

ONLY_FOR_ARCHS =	${APM_ARCHS}

COMMENT =		simple battery monitor for X

DISTNAME =		xbattmon-1.1
EPOCH=			23

CATEGORIES =		sysutils x11

HOMEPAGE =		https://git.2f30.org/xbattmon

# ISC
PERMIT_PACKAGE =	Yes

MASTER_SITES =		https://dl.2f30.org/releases/

WANTLIB =		X11 c

CONFIGURE_STYLE =	simple

MAKE_FLAGS = 		CFLAGS="${CFLAGS} -I${X11BASE}/include" \
			LDFLAGS="-L${X11BASE}/lib"
FAKE_FLAGS =		PREFIX="${PREFIX}"

NO_TEST =		Yes

post-patch:
	sed -i 's/blue/black/' ${WRKSRC}/config.def.h
	sed -i 's/green/black/' ${WRKSRC}/config.def.h
	sed -i 's/grey/black/' ${WRKSRC}/config.def.h
	sed -i 's/critical = 5/critical = 6/' ${WRKSRC}/config.def.h

.include <bsd.port.mk>
