# Maintainer: Gashon Husesin <gashon@ghussein.org>

pkgname=i3-lru
pkgver=1.0
pkgrel=1
pkgdesc="Provides an i3 LRU window switcher (daemon + rofi script)."
arch=('any')
url="https://github.com/gashon/i3-lru"
license=('MIT')
depends=('i3-wm' 'jq' 'rofi' 'bash')
source=('i3-lru.py'
	'i3-lru-daemon.sh'
	'i3-lru-daemon.service')
sha256sums=('SKIP' 'SKIP') # For local dev you can skip or fill real checksums

package() {
	cd "$srcdir"

	# Install the two scripts into /usr/bin
	install -Dm755 i3-lru "${pkgdir}/usr/bin/i3-lru"
	install -Dm755 i3-lru-daemon "${pkgdir}/usr/bin/i3-lru-daemon"

	# Optionally install docs like README.md
	# install -Dm644 README.md "${pkgdir}/usr/share/doc/${pkgname}/README.md"
}
