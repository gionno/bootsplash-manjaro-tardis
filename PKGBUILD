pkgbase=bootsplash-themes
pkgname=('bootsplash-theme-tardis')
pkgver=0.2
pkgrel=3
url="https://lists.freedesktop.org/archives/dri-devel/2017-December/160242.html"
arch=('x86_64')
license=('GPL')

depends=('systemd')
builddepends=('imagemagick')
options=('!libtool' '!emptydirs')

source=('bootsplash-packer'
	'bootsplash-theme-tardis.sh'
	'bootsplash-theme-tardis.initcpio_install'
	'tardis-spin.gif'
	'poweredby.png')

sha256sums=('SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP')

build() {
  cd "$srcdir"
  sh ./bootsplash-theme-tardis.sh
}

package_bootsplash-theme-tardis() {
  pkgdesc="Bootsplash Theme 'Tardis powered by'"
  cd "$srcdir"

  install -Dm644 "$srcdir/bootsplash-theme-tardis" "$pkgdir/usr/lib/firmware/bootsplash-themes/tardis/bootsplash"
install -Dm644 "$srcdir/bootsplash-theme-tardis.initcpio_install" "$pkgdir/usr/lib/initcpio/install/bootsplash-theme-tardis"
} 