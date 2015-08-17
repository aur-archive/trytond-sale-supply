# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-sale-supply
_pkgname=trytond_sale_supply
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The sale_supply module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-purchase>=3.4' 'trytond-sale>=3.4' 'trytond-stock>=3.4' 'trytond-stock-supply>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("3352e68ae7b66442756d66fd10e99e7e")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}