# Maintainer: Fr_nk <beat AT vi-di.fr>
pkgname=beat-time
pkgver=1.0
pkgrel=1
pkgdesc="Display the internet time, aka beat time"
arch=('x86_64' 'i686')
url="http://git.vi-di.fr/beat/"
license=('BSD')
depends=('glibc')
makedepends=('make')
provides=('beat')
conflicts=()
source=(http://git.vi-di.fr/beat/src/beat-${pkgver}.tar.gz)
sha256sums=('04529a591ab8cd54c8bc1182e30d8bac8f46275959ebd74d7b4848b66def967d')

build() {
  cd beat
  make
}

package() {
  cd beat
  make DESTDIR=${pkgdir} install
}
