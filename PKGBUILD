# Maintainer: Yurii Kolesnykov <root@yurikoles.com>
#
# PRs are welcome here: https://github.com/yurikoles-aur/obs-build
#

pkgname=obs-build
pkgver=20240612
pkgrel=1
license=(GPL-2.0-only GPL-3.0-only)
pkgdesc='OBS build script, can be used with OBS or stand alone'
url=https://github.com/openSUSE/obs-build
arch=(any)
depends=(perl)
source=("${pkgname}-${pkgver}.tar.gz::https://github.com/openSUSE/${pkgname}/archive/${pkgver}.tar.gz")
sha256sums=('ff9ab87a29291348d566f3305335fc245b051a2fbd63159287d855638d0aa9fd')

package() {
  cd "${pkgname}-${pkgver}"
  make DESTDIR="${pkgdir}" install
}
