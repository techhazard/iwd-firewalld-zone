# Maintainer: Vince van Oosten <techhazard@codeforyouand.me>
# Contributor: Rhys Perry <rhysperry111 AT gmail.com>
pkgname=iwd-firewalld-zone-git
_srcname=iwd-firewalld-zone
pkgver=1.0.0
pkgrel=1
pkgdesc='Automatically move wireless interface into firewalld zone based on setting in relevant iwd network file '
arch=(any)
url='https://github.com/techhazard/iwd-firewalld-zone'
license=('GPL-3.0-only')
depends=(systemd bash firewalld iwd gawk coreutils sed)
makedepends=(git)
provides=()
conflicts=()
install=PKGBUILD.install
source=('git+https://github.com/techhazard/iwd-firewalld-zone')
sha256sums=('SKIP')


pkgver() {
  cd "${_srcname}"
  git describe --long --tags --abbrev=7 | sed 's/\([^-]*-g\)/r\1/;s/-/./g'
}

package() {
	install -Dm 755 -t "${pkgdir}"/usr/bin/ "${_srcname}"/bin/*
	install -Dm 644 -t "${pkgdir}"/usr/lib/systemd/system/ "${_srcname}"/systemd/system/*
}
