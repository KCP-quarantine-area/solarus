pkgname="solarus-quest-editor"
pkgver="1.5.2"
pkgrel="1"
pkgdesc="A graphical user interface to create and modify quests for the Solarus engine."
arch=("x86_64")
url="http://www.solarus-games.org/"
license=("GPL" "custom")
depends=("solarus" "qt5-base" "qt5-tools")
makedepends=("cmake" "zip")
source=("https://github.com/solarus-games/$pkgname/archive/v$pkgver.tar.gz")
md5sums=("f20a6f50634d9d89a0657c21f53d5be6")

build() {
  cd "$srcdir/$pkgname-$pkgver"

  cmake -D CMAKE_BUILD_TYPE=Release -D CMAKE_INSTALL_PREFIX="/usr" .
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"

  make DESTDIR="${pkgdir}/" install
  install -Dm644 "license.txt" "$pkgdir/usr/share/licences/$pkgname/license.txt"
  install -Dm644 "images/logo/sqe-logo.png" "$pkgdir/usr/share/pixmaps/sqe-logo.png"
  install -Dm644 "resources/$pkgname.desktop" "$pkgdir/usr/share/applications/$pkgname.desktop"
}

