# Contributor: Nick B <Shirakawasuna at gmail _dot_com>
# Maintainer: Mark Coolen <mark dot coolen at gmail dot com>
pkgname=crosswordpuzzle
pkgver=1.0rc1
pkgrel=4
pkgdesc="A crossword puzzle game and editor."
arch=('i686' 'x86_64')
url="https://launchpad.net/crosswordpuzzle"
license=('GPL3')
depends=('gtk2' 'pygtk' 'python2')
source=(http://launchpad.net/"$pkgname"/1.0/"$pkgver"/+download/"$pkgname"-"$pkgver".tar.gz)
md5sums=('3699b1c8fadd232536d81c462a0749c7')

build() {

cd "$srcdir/$pkgname-$pkgver"
python2 setup.py build

}

package() {

cd "$srcdir/$pkgname-$pkgver"
python2 setup.py install --prefix="$pkgdir/usr"

}

