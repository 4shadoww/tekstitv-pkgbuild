# Maintainer: Noa-Emil Nissinen <aur dot easter at spamgourmet dot org>

pkgname=tekstitv
pkgver=0.9
pkgrel=1
pkgdesc="Yle tekstitv"
arch=('any')
url="https://github.com/Nykseli/yle-tekstitv"
license=('MIT')
source=("https://github.com/Nykseli/yle-tekstitv/archive/refs/tags/v$pkgver.tar.gz")
md5sums=("d9f6a7ac7ff86380f84c6f2930d845ba")


build(){
  cd yle-tekstitv-$pkgver
  ./configure --prefix=/usr --disable-lib-build
  make
}

package(){
  cd yle-tekstitv-$pkgver
  install -m 755 -D build/tekstitv $pkgdir/usr/bin/tekstitv
}
