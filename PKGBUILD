pkgname=messengerfordesktop
pkgver=v2.0.9
pkgrel=1
pkgdesc="Beautiful desktop client for Facebook Messenger. Chat without being distracted by your feed or notifications."
PKGEXT='.pkg.tar'
arch=('x86_64')
url="http://messengerfordesktop.com/"
license=('MIT')
options=(!strip)
depends=('cairo' 'gcc-libs' 'libxtst' 'alsa-lib' 'gtk2' 'gconf' 'libnotify' 'fontconfig' 'nss')
install=$pkgname.install
md5sums=('5c8862382e96c32a1878ce6f25a5b8da')
source=("https://github.com/Aluxian/Facebook-Messenger-Desktop/releases/download/$pkgver/Messenger_linux64.deb")
package() {
  bsdtar xf data.tar.gz
  chmod -R g-w opt
  chmod -R g-w usr
  mv opt "${pkgdir}"
  mv usr "${pkgdir}"
}
