#contributor: Francesco 'Kiko' Corsentino <kikocorsentino at gmail>
#contributor: ott <matthias.christian at tiscali.de>
#contributor: Ranguvar <ranguvar at archlinux.us>
#Maintainer: Daniel YC Lin <dlin.tw at gmail>

pkgname=bvi
pkgver=1.4.1
_pkgver=1.4.1
pkgrel=3
pkgdesc="A display-oriented editor for binary files operate like 'vi' editor"
url="http://bvi.sourceforge.net"
arch=(i686 x86_64)
depends=('ncurses')
license=("GPL")
source=('http://downloads.sourceforge.net/sourceforge/bvi/'$pkgname-$_pkgver'.src.tar.gz')

build ()
{
  cd "$srcdir/$pkgname-$_pkgver"
  ./configure --prefix=/usr --mandir=/usr/share/man
  make
}

package ()
{
  cd "$srcdir/$pkgname-$_pkgver"
  make DESTDIR="$pkgdir/" install
}
md5sums=('4d83d46e2ee76609a7b7b52e075a5900')
