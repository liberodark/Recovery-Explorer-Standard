# Maintainer: liberodark

pkgname=recovery-explorer-standard-6
pkgver=6.17.1
pkgrel=1
pkgdesc="Data Recovery Software."
arch=('x86_64')
url="https://www.sysdevlabs.com/order.php?prod=rxs6"
license=('Custom')
depends=('xdg-utils')
source_x86_64=("https://github.com/elcalc/elcalc/releases/download/4.8/elcalc_${pkgver}_amd64.deb")
source=(r-explorer.desktop
        r-explorer.png)
sha512sums=('32e16d5c74f462b8198ee52504f3cd997f72274b5eb35f2f420b3ea068fe317658c67165d08db3b52dc80bea8985a8e6378f794dd0e02d9cf989d99d1177ce9a'
         'bf660f725a340ef65e7ba1a781feeaaeaf26a68eb0097d2a24722b3017b124e38ae003fe184903afb1ac4c7cd36141fe0ec8057c930b5562c156b4be46a56831')
sha512sums_x86_64=('45ace5b62f30c6798c097ce7bffe2fd808cb67888c355bf036dc5bc75fdfc55761d6b0d2a17e04bdc611dcf5d2c00c1c0d07d335feb577d854b741de93374da2')
        
package() {
  cd $srcdir
  makedir recovery-explorer
  cp r-explorer $pkgdir/usr/lib/recovery-explorer/
  install -vDm644 $srcdir/$pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
  install -vDm644 $srcdir/$pkgname.png $pkgdir/usr/share/pixmaps/$pkgname.png
}

