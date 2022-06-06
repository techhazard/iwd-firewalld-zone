# Maintainer: Vince van Oosten <techhazard@codeforyouand.me>
pkgname=iwd-firewalld-zone
#pkgver=1.0.2
pkgver=0.1.0
pkgrel=1
epoch=
pkgdesc=""
arch=('any')
url="https://github.com/techhazard/${pkgname}"
license=('GPL3')
groups=()
depends=(systemd bash firewalld iwd gawk coreutils sed)
makedepends=(git)
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=PKGBUILD.install
changelog=
source=("${pkgname}.tgz::${url}/archive/refs/tags/${pkgver}.tar.gz")
validpgpkeys=()
sha256sums=('0915bfe7f907a05fbcf05b1ed84707f76e58c03548730aecc501f7f9f87d1496')


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
	src="${pkgname}-${pkgver}"
	install -D -m 755 -t $pkgdir/usr/bin/                "${src}"/bin/*
	install -D -m 644 -t $pkgdir/usr/lib/systemd/system/ "${src}"/systemd/system/*
}
