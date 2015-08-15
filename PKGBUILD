# $Id: PKGBUILD 78820 2012-10-25 06:47:28Z foutrelis $
# Maintainer: Sergej Pupykin <pupykin.s+arch@gmail.com>
# Contributor: William Rea <sillywilly@gmail.com>

pkgname=galago-daemon
pkgver=0.5.1
pkgrel=4
pkgdesc="Galago presence daemon"
arch=('i686' 'x86_64')
license=('GPL2')
url="http://www.galago-project.org"
depends=('libgalago')
source=(http://www.galago-project.org/files/releases/source/galago-daemon/galago-daemon-$pkgver.tar.gz)
md5sums=('fdb81f938f86f380b127158ebb542279')

build() {
  cd $srcdir/galago-daemon-$pkgver
  ./configure --prefix=/usr --sysconfdir=/etc --libexecdir=/usr/lib/$pkgname --disable-tests
  make
  make DESTDIR=$pkgdir install
}
