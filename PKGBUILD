# $Id: PKGBUILD 78820 2012-10-25 06:47:28Z foutrelis $
# Maintainer: Sven-Hendrik Haase <sh@lutzhaase.com>

pkgname=openarena-data
_pkgbasename=openarena
pkgver=0.8.8
_oldver=0.8.1
pkgrel=1
pkgdesc="A violent, sexy, multiplayer first person shooter based on the ioquake3 engine (data files)"
arch=('any')
url="http://openarena.ws/"
license=('GPL')
depends=()
makedepends=()
source=(http://download.tuxfamily.net/openarena/rel/081/oa081.zip
        http://download.tuxfamily.org/openarena/rel/085/oa085p.zip)
md5sums=('49006bcb02b4e8ea3d06749e8f4e4887'
         'b2a0437da751cd50dd2351ed9e0c4e9d')

build() {
    cd $srcdir/$_pkgbasename-$_oldver
}

package() {
    install -d $pkgdir/usr/share/$_pkgbasename/
    cp -rf $srcdir/$_pkgbasename-$_oldver/{baseoa,missionpack}/ $pkgdir/usr/share/$_pkgbasename/

    find $pkgdir/usr/share -type f -exec chmod 644 {} +
}

# vim: sw=2:ts=2 et:
