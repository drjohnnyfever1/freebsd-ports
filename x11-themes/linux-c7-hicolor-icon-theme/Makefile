# Created by: Piotr Kubaj <pkubaj@anongoth.pl>
# $FreeBSD$

PORTNAME=	hicolor-icon-theme
PORTVERSION=	0.5
PORTREVISION=	1
CATEGORIES=	x11-themes linux
MASTER_SITES=	# empty
DISTFILES=	# empty
PKGNAMEPREFIX=	linux-c7-

MAINTAINER=	emulation@FreeBSD.org
COMMENT=	High-color icon theme shell from the FreeDesktop project

CONFLICTS=	linux-c6-${PORTNAME}-[0-9]*

RUN_DEPENDS=	${LOCALBASE}/share/icons/hicolor/index.theme:misc/hicolor-icon-theme

NO_BUILD=	yes
USES=		linux:c7
USE_LINUX_PREFIX=	yes
PLIST_FILES=	usr/share/icons/hicolor

do-install:
	${INSTALL} -d ${STAGEDIR}${PREFIX}/usr/share/icons
	${LN} -fs ${LOCALBASE}/share/icons/hicolor ${STAGEDIR}${PREFIX}/usr/share/icons

.include <bsd.port.mk>
