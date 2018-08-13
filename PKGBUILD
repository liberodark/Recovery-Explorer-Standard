# Maintainer: liberodark

pkgname=recovery-explorer-standard-6
pkgver=6.17.1
pkgrel=1
pkgdesc="Data Recovery Software."
arch=('x86_64')
url="https://www.sysdevlabs.com/order.php?prod=rxs6"
license=('Custom')
depends=('xdg-utils')
source_x86_64=("r-explorer.tar.gz")
source=(r-explorer.desktop
        r-explorer.png)
sha512sums=('32e16d5c74f462b8198ee52504f3cd997f72274b5eb35f2f420b3ea068fe317658c67165d08db3b52dc80bea8985a8e6378f794dd0e02d9cf989d99d1177ce9a'
         'bf660f725a340ef65e7ba1a781feeaaeaf26a68eb0097d2a24722b3017b124e38ae003fe184903afb1ac4c7cd36141fe0ec8057c930b5562c156b4be46a56831')
sha512sums_x86_64=('0f6be28c56e7dcb5ec14e00d29771aa67a6493c2697e57d3c7156e183abae97d1e61ec72c60d553641ac5a35737c0b8a7b57430d6ed2b2a7db2fafcffa90342b')
        
package() {
  cd $srcdir
  tar xvf r-explorer.tar.gz
  mkdir -p "$pkgdir/usr/lib/recovery-explorer/"
  cp -r "r-explorer/." "$pkgdir/usr/lib/recovery-explorer/"
  install -vDm644 $srcdir/r-explorer.desktop $pkgdir/usr/share/applications/r-explorer.desktop
  install -vDm644 $srcdir/r-explorer.png $pkgdir/usr/share/pixmaps/r-explorer.png
  chmod +x "$pkgdir/usr/lib/recovery-explorer/r-explorer"
}