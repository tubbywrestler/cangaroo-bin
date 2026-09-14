# Maintainer: pineappletoad

pkgname=cangaroo-bin
pkgver=0.2.2.r64.gca7f907
_pkgrel_src=12
pkgrel=1
pkgdesc="Open source can bus analyzer software - with support for CANable / CANable2, CANFD, and other new features (precompiled)"
arch=('x86_64')
url="https://github.com/normaldotcom/cangaroo"
license=('GPL-2.0-only')
options=('!debug')
provides=('cangaroo')
conflicts=('cangaroo')
depends=(
    'bash'
    'gcc-libs'
    'glibc'
    'libnl'
    'qt5-charts'
    'qt5-base'
    'qt5-serialport'
)

source=("https://github.com/tubbywrestler/cangaroo-bin/releases/download/${pkgver}-${_pkgrel_src}/cangaroo-${pkgver}-${_pkgrel_src}-x86_64.pkg.tar.zst")
sha256sums=('967009255b2e4dfeed706579136687e9043498163cad10e8fb59f5af64bc6aa2')

package() {
    bsdtar -xf "${srcdir}/cangaroo-${pkgver}-${_pkgrel_src}-x86_64.pkg.tar.zst" -C "${pkgdir}" --exclude .PKGINFO --exclude .BUILDINFO --exclude .MTREE
}
