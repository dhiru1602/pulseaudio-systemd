# Maintainer: Dmitry Fillo <fillo at fillo dot me>
# Contributor: Joseph Lehner <joseph.c.lehner@gmail.com>

pkgname=pulseaudio-systemd
pkgver=1.1
pkgrel=1
epoch=
depends=(pulseaudio)
pkgdesc='A systemd service for running PulseAudio in system-wide mode'
arch=(any)
url='http://www.freedesktop.org/wiki/Software/PulseAudio/Documentation/User/WhatIsWrongWithSystemWide'
license=('GPL')
install=install
source=(pulseaudio.service pulseaudio-system-wide.conf)
md5sums=('7740ba866ecb74d708baaebb9328640d'
         '194fc7b6b88d81194fe4ae1a9ca0fff4')

package() {
  install -m 644 -D pulseaudio.service "$pkgdir/"usr/lib/systemd/system/pulseaudio.service
  install -m 644 -D pulseaudio-system-wide.conf "$pkgdir/"etc/dbus-1/system.d/pulseaudio-system-wide.conf
}
