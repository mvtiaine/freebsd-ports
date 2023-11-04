PORTNAME=	audacious-uade
PORTVERSION=	0.9.2
CATEGORIES=	multimedia audio

GH_ACCOUNT=	mvtiaine
MASTER_SITES=	GHC/releases/download/${DISTVERSION}/

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

.include <bsd.port.mk>
