# Created by: Johannes Meixner <xmj@chaot.net>
# $FreeBSD$

PORTNAME=	cups-libs
PORTVERSION=	1.4.2
CATEGORIES=	print linux

MAINTAINER=	emulation@FreeBSD.org
COMMENT=	Common UNIX Printing System libraries

USE_LINUX=	yes
USE_LINUX_RPM=	yes
USE_LINUX_APPS=	gnutls
SRC_DISTFILES=	cups-${PORTVERSION}-${RPMVERSION}.src.rpm
LINUX_DIST_VER=	10
RPMVERSION=	50.el6_4.5
USE_LDCONFIG=	yes

PLIST_FILES=	usr/lib/libcups.so.2 usr/lib/libcupscgi.so.1 usr/lib/libcupsdriver.so.1 \
			   	usr/lib/libcupsimage.so.2 usr/lib/libcupsmime.so.1 usr/lib/libcupsppdc.so.1
DESCR=		${.CURDIR}/../cups-base/pkg-descr

.include <bsd.port.mk>
