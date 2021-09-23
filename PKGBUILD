# Maintainer: prometheansacrifice <prometheansacrifice@gmail.com>
pkgname='esy-nightly'
pkgver='0.6.11+nightly'
arch=('i686' 'x86_64')
pkgrel='1'
pkgdesc="Development builds of esy - a package manager for OCaml/Reason"
url="https://esy.sh/"
license=('MIT')
depends=('bash' 'git' 'gcc-libs' 'npm')
conflicts=('esy')
_npmname=@esy-nightly/esy

package() {
  npm install -g --prefix "$pkgdir/usr" $_npmname
}

pre_remove() {
  npm remove -g $_npmname
}
