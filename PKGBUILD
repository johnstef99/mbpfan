# Maintainer: John Stef <john@johnstef.com>

pkgname=mbpfan
pkgver=1.2
pkgrel=1
pkgdesc="Automatically adjust the fan on a MacBook Pro"
arch=('i686' 'x86_64')
license=('GPL3')
source=(mbpfan.c 
        mbpfan.service)
md5sums=('f42e5b1de8cbf389ddfc6231991e9c34'
         '4d106907fcae64ebd0418428eff12c79')

build() {
  cd $srcdir/
  gcc -o mbpfan -lm -Wall $CFLAGS $LDFLAGS mbpfan.c
}

package() {
  install -Dm755 $srcdir/mbpfan $pkgdir/usr/bin/mbpfan
  install -Dm755 $srcdir/mbpfan.service $pkgdir/etc/systemd/system/mbpfan.service
}
