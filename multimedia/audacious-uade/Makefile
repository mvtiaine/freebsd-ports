PORTNAME=	audacious-uade
PORTVERSION=	0.12.3
CATEGORIES=	multimedia audio

MASTER_SITES=	https://github.com/mvtiaine/audacious-uade/releases/download/${DISTVERSION}/

COMMENT=	UADE plugin for Audacious music player
WWW=		https://github.com/mvtiaine/audacious-uade

LICENSE=	GPLv2+
LICENSE_FILE=	${WRKSRC}/COPYING

RUN_DEPENDS=	audacious:multimedia/audacious

GNU_CONFIGURE=	yes
CONFIGURE_ARGS=	--enable-plugin-audacious=yes --with-static-stdlibs=no
USES=	compiler:c++11-lib gmake pkgconfig tar:bz2
TEST_TARGET=	check

.include <bsd.port.mk>
