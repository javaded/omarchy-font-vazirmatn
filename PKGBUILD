# Maintainer: JED j.effatdoost@gmail.com
pkgname=omarchy-font-vazirmatn
pkgver=1.0
pkgrel=1
pkgdesc="Vazirmatn Persian font with fontconfig rules for Omarchy (variable font)"
arch=('any')
url="https://github.com/javaded/omarchy-font-vazirmatn.git"
license=('OFL-1.1')
depends=('fontconfig' 'noto-fonts')
source=(
  "Vazirmatn-VariableFont_wght.ttf"
  "20-persian.conf"
  "LICENSE"
)
sha256sums=(
  '700c63e8f904d7519f3e8f33dfe90edae403e48054a86d33c0b671518a079838'
  'a9e96912ba182d62d314cdbaa81572dda632d3d724bb3bc19cd059065da78689'
  'ac7d96cb9100b87ce25d02becf2264d7502c1638ca23f270f034ef3bc0eaa01d'
)

package() {
  # Create directories
  install -d "$pkgdir/usr/share/fonts/TTF"
  install -d "$pkgdir/etc/fonts/conf.d"
  install -d "$pkgdir/usr/share/licenses/$pkgname"

  # Install font
  install -m644 Vazirmatn-VariableFont_wght.ttf "$pkgdir/usr/share/fonts/TTF/"

  # Install fontconfig rule
  install -m644 20-persian.conf "$pkgdir/etc/fonts/conf.d/"

  # Install license
  install -m644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
