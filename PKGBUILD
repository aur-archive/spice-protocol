# Maintainer: Patryk Kowalczyk < patryk at kowalczyk dot ws> 

pkgname=spice-protocol
pkgver=0.12.6
pkgrel=1
pkgdesc="Headers for SPICE protocol."
arch=(any)
url="http://spice-space.org"
license=('GPL')
source=(http://spice-space.org/download/releases/$pkgname-$pkgver.tar.bz2)

build() {
  cd "$srcdir/$pkgname-$pkgver"
  PYTHON=python2 \
  ./configure --prefix=/usr
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"

  make DESTDIR="$pkgdir/" install
}

md5sums=('797d18156ab893e48778cb097b21bb2b')
