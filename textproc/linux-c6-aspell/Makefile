# Created by: Johannes Meixner <xmj@chaot.net>
# $FreeBSD$

PORTNAME=	aspell
PORTVERSION=	0.60.6
CATEGORIES=	textproc linux

MAINTAINER=	emulation@FreeBSD.org
COMMENT=	Spelling checker with better logic than ispell (Linux CentOS ${LINUX_DIST_VER})

CONFLICTS=	linux-aspell-[0-9]* linux-f10-aspell-[0-9]*

ONLY_FOR_ARCHS=	i386 amd64
USE_LINUX=	yes
USE_LINUX_RPM=	yes

RPMVERSION=	12.el6
BRANDELF_DIRS=	usr/bin
USE_LDCONFIG=	yes

DESCR=		${.CURDIR}/../${PORTNAME}/pkg-descr

.include <bsd.port.mk>
