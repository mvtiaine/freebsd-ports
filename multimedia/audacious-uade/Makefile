PORTNAME=	audacious-uade
PORTVERSION=	0.14.0
CATEGORIES=	multimedia audio

MASTER_SITES=	https://github.com/mvtiaine/audacious-uade/releases/download/${DISTVERSION}/

COMMENT=	UADE plugin for Audacious and DeaDBeeF
WWW=		https://github.com/mvtiaine/audacious-uade

LICENSE=	GPLv2+
LICENSE_FILE=	${WRKSRC}/COPYING

LIB_DEPENDS=	libopenmpt.so:audio/libopenmpt \
                libxmp.so:audio/libxmp
RUN_DEPENDS=	audacious:multimedia/audacious
BUILD_DEPENDS=	audacious:multimedia/audacious

GNU_CONFIGURE=	yes
CONFIGURE_ARGS=	--enable-players=all --enable-plugin-audacious=yes --with-static-stdlibs=no
USES=	compiler:c++11-lib gmake pkgconfig tar:bz2
TEST_TARGET=	check

# DeaDBeeF >= 1.8.0 required
#OPTIONS_DEFINE=	DEADBEEF
#DEADBEEF_CONFIGURE_ENABLE=	plugin-deadbeef=yes
#DEADBEEF_RUN_DEPENDS=	deadbeef:audio/deadbeef
#DEADBEEF_BUILD_DEPENDS=	deadbeef:audio/deadbeef
CONFIGURE_ARGS+=	--enable-plugin-deadbeef=no

.include <bsd.port.mk>
