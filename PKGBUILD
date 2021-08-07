#contributor: Francesco 'Kiko' Corsentino <kikocorsentino at gmail>
#contributor: ott <matthias.christian at tiscali.de>
#contributor: Ranguvar <ranguvar at archlinux.us>
#Maintainer: Daniel YC Lin <dlin.tw at gmail>

pkgname=bvi
pkgver=1.4.1_relgoto
_pkgver=1.4.1_relgoto
pkgrel=3
pkgdesc="A display-oriented editor for binary files operate like 'vi' editor"
url="http://bvi.sourceforge.net"
arch=(i686 x86_64)
depends=('ncurses')
license=("GPL")
source=('bvi::git+https://github.com/krafczyk/bvi#rel_goto')

build ()
{
  cd "$srcdir/bvi"
  ./configure --prefix=/usr --mandir=/usr/share/man
  make
}

package ()
{
  cd "$srcdir/bvi"
  make DESTDIR="$pkgdir/" install
}
