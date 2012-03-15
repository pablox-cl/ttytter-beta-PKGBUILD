# Maintainer: Pablo Olmos de Aguilera <pablo at glatelier dot org>
# Contributor: TDY <tdy at gmx dot com>
# Contributor: Roberto Viola <cagnulein at gmail dot com>

pkgname=ttytter-beta
pkgver=2.0.0b6
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
md5sums=('056779f62628b5d16bf1b4a36c6fb71d'
         '14d9fd6cc89ac7142b205cff213cb581')
build() {
  cd "$srcdir"
  install -Dm755 $_pkgver.txt "$pkgdir/usr/bin/$pkgname"
  install -Dm644 license.txt "$pkgdir/usr/share/licenses/$pkgname/license.txt"
}
