# Created by: msmith@FreeBSD.org
# $FreeBSD$

PORTNAME=	linux_kdump
PORTVERSION=	1.5
PORTREVISION=	333
CATEGORIES=	devel linux
MASTER_SITES=	${MASTER_SITE_LOCAL}
MASTER_SITE_SUBDIR=	marcel

MAINTAINER=	emulation@FreeBSD.org
COMMENT=	Linux-compatibility ktrace.out processor

USE_LINUX=	yes
USE_LINUX_APPS=	devtools
BUILD_DEPENDS=	${RUN_DEPENDS} # USE_LINUX_APPS only sets RUN_DEPENDS

ONLY_FOR_ARCHS=	i386 amd64
NO_MANCOMPRESS=	yes
PLIST_FILES=	bin/linux_kdump man/man1/linux_kdump.1.gz

.include <bsd.port.pre.mk>

pre-everything::
	@${ECHO_MSG} '===> Using the FreeBSD source tree under ${SRC_BASE}'
	@${ECHO_MSG} '===> Set SRC_BASE to use an alternate source tree'

.if !exists(${SRC_BASE}/sys/i386/linux/syscalls.master)
IGNORE=	requires kernel source present in ${SRC_BASE}/sys
.endif
.if !exists(${SRC_BASE}/usr.bin/ktrace/subr.c)
IGNORE=	requires ktrace source present in ${SRC_BASE}/usr.bin/ktrace
.endif
.if ! (exists(${LINUXBASE}/etc/fedora-release) || exists(${LINUXBASE}/etc/centos-release))
IGNORE=	does not build without a linux base, use the package instead
.endif

.include <bsd.port.post.mk>
