# Maintainer: Hugo Posnic <hugo.posnic@gmail.com>
# Author: Hugo Posnic <hugo.posnic@gmail.com>
# Author: Nathan Seva <nathan.seva@outlook.fr>
pkgname=imeditor
pkgver=0.1.1
pkgrel=1
pkgdesc="Simple & versatile image editor."
arch=("any")
url="https://github.com/ImEditor/ImEditor"
license=('GPL')
depends=('python' 'gtk3' 'python-pillow')
source=("$url/archive/$pkgver.tar.gz")
md5sums=("3090bb9a30b26bd9be6339a0d950b3df")

package() {
    cd ${srcdir}/ImEditor-$pkgver
    install -dm755 ${pkgdir}/usr/share/${pkgname}
    cp -R imeditor/* ${pkgdir}/usr/share/${pkgname}
    install -D -m644 ${pkgname}.desktop ${pkgdir}/usr/share/applications/${pkgname}.desktop
}
