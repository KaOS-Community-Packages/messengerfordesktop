pkgname=messengerfordesktop
pkgver=2.0.9
pkgrel=1
pkgdesc="Beautiful desktop client for Facebook Messenger. Chat without being distracted by your feed or notifications."
PKGEXT='.pkg.tar'
arch=('x86_64')
url="http://messengerfordesktop.com/"
license=('MIT')
options=(!strip)
depends=('cairo' 'gcc-libs' 'libxtst' 'alsa-lib' 'gtk2' 'gconf' 'libnotify' 'fontconfig' 'nss')
install=$pkgname.install
source=("https://github.com/Aluxian/Facebook-Messenger-Desktop/releases/download/v${pkgver}/messengerfordesktop-${pkgver}-linux-amd64.deb")
sha512sums=('76c4a891e795d9b0fdf8efa17cf5ffa475a9d522f05d944116f605f189425df583a8f8928755172142b5751d289d2bd67c7952d5132fb12d1939b5f86e781a7f')

package() {
  bsdtar xf data.tar.gz
  chmod -R g-w opt
  chmod -R g-w usr
  mv opt "${pkgdir}"
  mv usr "${pkgdir}"
}
