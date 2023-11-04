PORTNAME=	audacious-uade
PORTVERSION=	0.9.3
CATEGORIES=	multimedia audio

MASTER_SITES=	https://github.com/mvtiaine/audacious-uade/releases/download/${DISTVERSION}/

COMMENT=	UADE plugin for Audacious music player
WWW=		https://github.com/mvtiaine/audacious-uade

LICENSE=	GPLv2+
LICENSE_FILE=	${WRKSRC}/COPYING

RUN_DEPENDS=	audacious:multimedia/audacious

GNU_CONFIGURE=	yes
USES=	compiler:c++11-lib gmake pkgconfig tar:bz2
# CC must be set if using clang, as UADE submodule configure fails otherwise
CC?=	clang
CXX?=	clang++

.if defined(WITH_DEBUG)
INSTALL_TARGET=install
.else
INSTALL_TARGET=install-strip
.endif

.include <bsd.port.mk>
