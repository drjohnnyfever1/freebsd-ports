# Created by: Piotr Kubaj <pkubaj@anongoth.pl>
# $FreeBSD$

PORTNAME=	alsa-plugins-oss
PORTVERSION=	1.1.1
CATEGORIES=	audio linux

MAINTAINER=	emulation@FreeBSD.org
COMMENT=	OSS plugin for ALSA (Linux CentOS ${LINUX_DIST_VER})

LICENSE=	GPLv3

CONFLICTS=	linux-c6-${PORTNAME}-[0-9]*

SRC_DISTFILES=	alsa-plugins-${PORTVERSION}-${RPMVERSION}${SRC_SUFX}:SOURCE

RPMVERSION=	1.el7
USES=		linux:c7
USE_LDCONFIG=	yes
USE_LINUX=	alsalib
USE_LINUX_RPM=	yes

# We will use native configuration file, so delete a linux one
post-extract:
	@${RM} -r ${WRKSRC}/etc

.include <bsd.port.mk>
