# Created by: peter
# $FreeBSD: head/security/linux-f10-cyrus-sasl2/Makefile 340722 2014-01-22 17:00:46Z mat $

PORTNAME=	cyrus-sasl2
PORTVERSION=	2.1.22
PORTREVISION=	2
CATEGORIES=	security linux
MASTER_SITES=	CRITICAL/rpm/${LINUX_RPM_ARCH}/fedora/${LINUX_DIST_VER}
DISTNAME=	cyrus-sasl-lib-${PORTVERSION}-${RPMVERSION}

SRC_DISTFILES=	cyrus-sasl-${PORTVERSION}-${RPMVERSION}.src.rpm

MAINTAINER=	emulation@FreeBSD.org
COMMENT=	RFC 2222 SASL (Simple Authentication and Security Layer) (Linux Fedora 10)

USE_LINUX=	f10
USE_LINUX_RPM=	yes

RPMVERSION=	19.fc10
USE_LDCONFIG=	yes
BRANDELF_FILES=	usr/sbin/sasldblistusers2 usr/sbin/saslpasswd2
DESCR=	${.CURDIR}/../${PORTNAME}/pkg-descr

PLIST_DIRS=	etc/sasl2 usr/lib/sasl2
PLIST_FILES=	usr/lib/libsasl2.so.2 usr/lib/libsasl2.so.2.0.22 usr/lib/sasl2/libanonymous.so usr/lib/sasl2/libanonymous.so.2 usr/lib/sasl2/libanonymous.so.2.0.22 usr/lib/sasl2/libsasldb.so usr/lib/sasl2/libsasldb.so.2 usr/lib/sasl2/libsasldb.so.2.0.22 usr/sbin/sasldblistusers2 usr/sbin/saslpasswd2
PLIST_FILES+=	"@exec mkdir -p %D/etc/sasl2"
DOCSDIR=	usr/share/doc/cyrus-sasl-lib-${PORTVERSION}
PORTDOCS=	AUTHORS COPYING NEWS README advanced.html appconvert.html components.html gssapi.html index.html install.html macosx.html mechanisms.html options.html plugprog.html programming.html readme.html sysadmin.html upgrading.html windows.html

.include <bsd.port.mk>
