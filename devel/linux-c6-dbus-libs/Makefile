# Created by: Artyom Mirgorodskiy <artyom.mirgorodsky@gmail.com>
# $FreeBSD$

PORTNAME=	dbus-libs
PORTVERSION=	1.2.24
CATEGORIES=	devel linux

MAINTAINER=	emulation@FreeBSD.org
COMMENT=	Libraries for accessing D-BUS (Linux CentOS ${LINUX_DIST_VER})

ONLY_FOR_ARCHS=	i386 amd64
USE_LINUX=	yes

.if defined(PACKAGE_BUILDING)
SRC_DISTFILES=	dbus-1.2.24-7.el6_3.src.rpm
.endif

USE_LINUX_RPM=	yes
RPMVERSION=	7.el6_3
USE_LDCONFIG=	yes
DESCR=		${.CURDIR}/../dbus/pkg-descr

PLIST_FILES=	lib/libdbus-1.so.3 lib/libdbus-1.so.3.4.0

CONFLICTS=	linux-dbus-libs-[0-9]*  linux-f10-dbus-libs-[0-9]*

.include <bsd.port.mk>
