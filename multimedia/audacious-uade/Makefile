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

.include <bsd.port.mk>
