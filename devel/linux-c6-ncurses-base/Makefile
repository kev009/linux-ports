# Created by: Johannes Meixner <xmj@chaot.net>
# $FreeBSD$

PORTNAME=	${LINUX_NAME}-base
PORTVERSION=	5.7
CATEGORIES=	devel linux

MAINTAINER=	jwbacon@tds.net
COMMENT=	Terminfo database required by Linux ncurses programs

USE_LINUX=	yes
USE_LINUX_RPM=	yes
LINUX_NAME=	ncurses

RPMVERSION=	3.20090208.el6
SRC_DISTFILES=	${LINUX_NAME}-${PORTVERSION}-${RPMVERSION}${SRC_SUFX}
DESCR=	${.CURDIR}/../${LINUX_NAME}/pkg-descr

.include <bsd.port.mk>
