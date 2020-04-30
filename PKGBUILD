pkgbase=bootsplash-themes
pkgname=('bootsplash-theme-manjaro-globe')
pkgver=1
pkgrel=1
url="https://lists.freedesktop.org/archives/dri-devel/2017-December/160242.html"
arch=('x86_64')
license=('GPL')

depends=()
builddepends=('imagemagick')
options=('!libtool' '!emptydirs')

source=('bootsplash-packer'
	'bootsplash-manjaro-globe.sh'
	'bootsplash-manjaro-globe.initcpio_install'
	'spinner.gif'
	'logo.png')

sha256sums=('SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP')

build() {
  cd "$srcdir"
  sh ./bootsplash-manjaro-globe.sh
}

package_bootsplash-theme-manjaro-globe() {
  pkgdesc="Bootsplash Theme Manjaro Globe"
  cd "$srcdir"

  install -Dm644 "$srcdir/bootsplash-manjaro-globe" "$pkgdir/usr/lib/firmware/bootsplash-themes/manjaro-globe/bootsplash"
  install -Dm644 "$srcdir/bootsplash-manjaro-globe.initcpio_install" "$pkgdir/usr/lib/initcpio/install/bootsplash-manjaro-globe"
} 
