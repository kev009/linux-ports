# Created by: Johannes Meixner <xmj@chaot.net>
# $FreeBSD$

PORTNAME=	tcl
PORTVERSION=	8.5.7
CATEGORIES=	lang linux
PKGNAMESUFFIX=	85

MAINTAINER=	emulation@FreeBSD.org
COMMENT=	Tool Command Language (Linux CentOS ${LINUX_DIST_VER})

# XXX: someone should make libarchive be quiet about symlinks
EXTRACT_DEPENDS=	rpm2cpio.pl:${PORTSDIR}/archivers/rpm2cpio

EXTRACT_CMD=	rpm2cpio.pl
EXTRACT_BEFORE_ARGS:=
EXTRACT_AFTER_ARGS=	| cpio -idm --insecure

CONFLICTS=	linux-f10-tcl85-[0-9]*

ONLY_FOR_ARCHS=	i386 amd64

USE_LINUX=	yes
USE_LINUX_RPM=	yes
RPMVERSION=	6.el6
BRANDELF_FILES=	usr/bin/tclsh usr/bin/tclsh8.5
USE_LDCONFIG=	yes
NO_WRKSUBDIR=	yes

DESCR=		${.CURDIR}/../${PORTNAME}${PKGNAMESUFFIX}/pkg-descr

.include <bsd.port.mk>
