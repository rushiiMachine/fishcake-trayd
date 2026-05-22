pkgname=fishcake-trayd
pkgver=1.0.0
pkgrel=1
pkgdesc="Persistent fishcake tray icon"
url="https://github.com/rushiiMachine/fishcake-trayd"
license=('GPL3')

arch=('any')
depends=(
    'python3'
    'gtk3'
    'libayatana-appindicator'
)
optdepends=(
    'gnome-shell-extension-appindicator: Tray icons support for gnome-shell'
)

install=fishcake-trayd.install

source=(
    "${pkgname}"
    "${pkgname}.service"
    "fishcake-tray.svg"
)
sha256sums=('64ce606d4d47de817f602a9456dfc395ca2299f3ea8357760a25ca46b62fe924'
            '9bf1cab95deb3cfc3126de81856303019499926ea069dad6362cc4b80040d73b'
            '9b91a0f778c4072c4446599a6e62e42d5c107bd735db8783eaf5377ad666ba28')

package() {
    install -Dm755 "${pkgname}" "$pkgdir/usr/bin/${pkgname}"
    install -Dm644 "${pkgname}.service" "$pkgdir/usr/share/systemd/user/${pkgname}.service"
    install -Dm644 "fishcake-tray.svg" "$pkgdir/usr/share/icons/hicolor/scalable/status/fishcake-tray.svg"
}
