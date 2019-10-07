# Created by: Kris Moore <kris@ixsystems.com>
# $FreeBSD$

PORTNAME=	pc-networkmanager
PORTVERSION=	201907311200
CATEGORIES=	sysutils

MAINTAINER=	kris@ixsystems.com
COMMENT=	TrueOS Qt based network manager

LICENSE=	BSD2CLAUSE

LIB_DEPENDS=	libtrueos-ui.so:sysutils/trueos-libqt5

MAKE_ARGS=      PREFIX=${STAGEDIR}${PREFIX}

CONFLICTS=      pcbsd-utils*

MAKE_JOBS_UNSAFE=yes
ONLY_FOR_ARCHS= amd64
USE_LDCONFIG=   yes
USES=	qt:5 qmake shebangfix tar:xz
USE_QT=        core gui network svg linguist \
		buildtools x11extras widgets
USE_GL+=	gl

QMAKE_ARGS=     CONFIG+="configure"

USE_GITHUB=	yes
GH_ACCOUNT=	project-trident
GH_PROJECT=	pc-networkmanager
GH_TAGNAME=	4105d294e51c459ee93205d5fa52d9e037a9b89b

.include <bsd.port.mk>
