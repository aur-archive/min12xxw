# Contributor: Martin Tuma <tumic@cbox.cz>
pkgname=min12xxw
pkgver=0.0.9
pkgrel=2
pkgdesc="Minolta PagePro 1[234]xxW printers driver"
url="http://www.hinterbergen.de/mala/min12xxw/"
arch=('i686' 'x86_64')
license=('GPL')
depends=('foomatic-db')
source=('http://www.hinterbergen.de/mala/min12xxw/min12xxw-0.0.9.tar.gz')
md5sums=('3582da7bd8d2d612b1fbcbfdb8b3239a')

build() {
  cd "$pkgname-$pkgver"
  ./configure --prefix=/usr
  make
}

package() {
  cd "$pkgname-$pkgver"
  make DESTDIR="$pkgdir/" install
}

# vim:syntax=sh
