# Maintainer: Eric Bailey <nerflad@gmail.com>
pkgname=sloc
pkgver=0.3.2
pkgrel=1
pkgdesc='Simple source-lines-of-code counter'
arch=('i686' 'x86_64')
url="http://git.bytbox.net/sloc/"
license=('MIT')
makedepends=('git' 'go')
source=("sloc::git+https://github.com/nerflad/sloc.git")
md5sums=('SKIP')

build() {
  cd ${srcdir}/sloc
  go build -o sloc
}

package() {
  cd ${srcdir}
  install -Dm755 sloc/sloc "$pkgdir"/usr/bin/sloc
}
