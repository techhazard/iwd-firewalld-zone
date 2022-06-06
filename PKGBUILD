# Maintainer: Vince van Oosten <techhazard@codeforyouand.me>
pkgname=iwd-firewalld-zone
pkgver=0.1.0
pkgrel=1
epoch=
pkgdesc=""
arch=('any')
url="https://github.com/techhazard/${_pkgname}"
license=('GPL3')
groups=()
depends=(systemd bash firewalld iwd awk grep coreutils)
makedepends=(git)
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("$pkgname::git+${url}.git#tag=${pkgver}")
noextract=()
md5sums=()
validpgpkeys=()

prepare() {
	true
}

build() {
	true
}

check() {
	true
}

package() {
	install -d ${pkgdir}/usr/lib/systemd/system/iwd-firewalld-zone.target.wants/
	install -D -m 755 -t $pkgdir/usr/bin/ iwd-firewalld-zone
	install -D -m 644 -t $pkgdir/usr/lib/systemd/system/ iwd-firewalld-zone@.service iwd-firewalld-zone.{path,target}
}
