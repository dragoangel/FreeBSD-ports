# Created by: Olivier Duchateau <duchateau.olivier@gmail.com>
# $FreeBSD$

PORTNAME=	bjoern
PORTVERSION=	3.1.0
CATEGORIES=	www python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	python@FreeBSD.org
COMMENT=	Fast Python WSGI server

LICENSE=	BSD2CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

LIB_DEPENDS=	libev.so:devel/libev

USES=		localbase python
USE_PYTHON=	autoplist concurrent distutils

LDFLAGS+=	-lc

post-install:
	${STRIP_CMD} ${STAGEDIR}${PYTHON_SITELIBDIR}/*.so

.include <bsd.port.mk>
