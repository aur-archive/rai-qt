# Contributor: 

pkgname=rai-qt
pkgver=0.3.2
pkgrel=1
pkgdesc="This script uses kdialog to generate a list of italian rai's channels"
arch=('any')
url="http://www.kde-apps.org/content/show.php/Rai-qt?content=112093"
license=('GPL')
depends=('kdebase-kdialog' 'kdesdk-kate' 'kdebase-konqueror' 'vlc')
source=(http://www.kde-apps.org/CONTENT/content-files/112093-${pkgname})
md5sums=('4d71564582de999964a5bd6eae9b55d5')

build() {
  sed -i -e "s:/usr/local:/usr:g" 112093-rai-qt
  sed -i -e "s:kdesudo:kdesu:g" 112093-rai-qt
  install -Dm755 ${srcdir}/112093-${pkgname} "${pkgdir}/usr/bin/${pkgname}" || return 1
}
