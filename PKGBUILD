# Maintainer: Megameneer (Dennis Holierhoek) <dennis.hh@hotmail.com>
pkgname=esrpatch
pkgver=02
pkgrel=4
# This line is way over 80 characters, but a clear description for this rather specific tool is hard to make any shorter than this.
pkgdesc="A tool to patch DVD disc images for the Sony PlayStation 2 game console to make them burnable and working with ESR, an app for the PlayStation 2 made to play those burned games without swapping"
arch=('any')
url=https://github.com/antipatico/esr-disc-patcher-cli
license=('GPL')
depends=()
makedepends=('w3m')
source=('git+https://github.com/antipatico/esr-disc-patcher-cli.git#branch=C++11')
md5sums=('SKIP')

build() {
	cd "$srcdir"/esr-disc-patcher-cli
	make
}

package() {
	cd "$srcdir"/esr-disc-patcher-cli
	install -D esrpatch "$pkgdir"/usr/bin/esrpatch
}
