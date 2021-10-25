# Maintainer: Husam Bilal <me@husam.dev>

pkgname=cliphist
pkgver=0.2.0
pkgrel=1
pkgdesc="clipboard history 'manager' for wayland"
url="https://github.com/sentriz/cliphist"
depends=("wl-clipboard>=2.0" "xdg-utils")
makedepends=("go")
provides=("cliphist")
license=("GPL3")
arch=("x86_64" "aarch64")
md5sums=("3d58113e42c73b452dc5655459bd0d34")
source=("https://github.com/sentriz/${pkgname}/archive/v${pkgver}.tar.gz")

build() {
  cd $pkgname-$pkgver
  go build .
}

package() {
  cd $pkgname-$pkgver
  install -Dm755 $pkgname $pkgdir/usr/bin/$pkgname
}
