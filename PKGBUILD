# Maintainer: Pablo Olmos de Aguilera <pablo at glatelier dot org>

pkgname=ttytter-beta
pkgver=2.0.0b7
_pkgver=beta
pkgrel=1
pkgdesc="A multi-functional, command-line twitter client; beta version"
arch=('any')
url="http://www.floodgap.com/software/ttytter/beta/"
license=('custom:FFSL')
depends=('perl')
optdepends=('perl-datetime-format-dateparse'
            'perl-term-readline'
            'perl-term-readline-ttytter: For automatic prompt updating, history
            synchronization, background control and character counter.')
source=(http://www.floodgap.com/software/ffsl/license.txt
        $_pkgver.txt::http://www.floodgap.com/software/ttytter/beta/$_pkgver.txt)
sha256sums=('42c576fcacb5bd6c8f8e64c479b0f8e4445c7e6c9ac013485c51b8f05f2352fd'
            '5fb21aefb8ffd8bfc11b626efb232e9356c3852968961e60299d009925ceba13')

build() {
  return 0
}

package() {
  cd "$srcdir"
  install -Dm755 $_pkgver.txt "$pkgdir/usr/bin/$pkgname"
  install -Dm644 license.txt "$pkgdir/usr/share/licenses/$pkgname/license.txt"
}
