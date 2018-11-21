pkgname=soulseekqt
pkgver=20160117
_pkgver=2016-1-17-64bit
pkgrel=1
pkgdesc="A desktop client for the Soulseek peer-to-peer file sharing network"
arch=('x86_64')
license=('custom')
url="http://www.soulseekqt.net/news/"
depends=('libxext' 'fontconfig' 'libxrender')
md5sums=('c843e748a129e4ad9461280aeb2b957a'
         '16f9bfbb52c375a8143d4b164a7ec995'
         '256ec24f7ad2d39ac8da0f1c03d3cafe')

source=("https://www.dropbox.com/s/7qh902qv2sxyp6p/SoulseekQt-2016-1-17-64bit.tgz?dl=0"
        $pkgname.desktop 
        $pkgname.png)

package() {
  install -vDm755 "$srcdir/SoulseekQt-$_pkgver" "$pkgdir/usr/bin/$pkgname"
  install -vDm644 "$srcdir/$pkgname.desktop" "$pkgdir/usr/share/applications/$pkgname.desktop"
  install -vDm644 "$srcdir/$pkgname.png" "$pkgdir/usr/share/pixmaps/$pkgname.png"
}
