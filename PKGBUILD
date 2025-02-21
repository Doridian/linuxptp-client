# Maintainer: Doridian <archlinux at doridian dot net>

pkgname=linuxptp-client
pkgver=1.0
pkgrel=1
pkgdesc='Configure LinuxPTP as a client'
arch=('any')
url='https://github.com/Doridian/linuxptp-client.git'
license=('MIT')
depends=('linuxptp')
source=(
    'ptp4l.service'
    'phc2sys.service'
    'ptp4l.conf'
    'ptp4l.env'
)
sha256sums=(
    'SKIP'
    'SKIP'
    'SKIP'
    'SKIP'
)

build() {
    echo OK
}

package() {
    cd "${srcdir}"
    install -Dm644 ptp4l.service "${pkgdir}/etc/systemd/system/ptp4l.service"
    install -Dm644 phc2sys.service "${pkgdir}/etc/systemd/system/phc2sys.service"
    install -Dm644 ptp4l.conf "${pkgdir}/etc/ptp4l.conf"
    install -Dm644 ptp4l.env "${pkgdir}/etc/ptp4l.env"
}

# vim:set ts=2 sw=2 et:
