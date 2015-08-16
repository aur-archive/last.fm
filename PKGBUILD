# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Brandon <bwaynej2002@embarqmail.com>
pkgname=last.fm
pkgver=1.5.4.26862
pkgrel=2
#epoch=
pkgdesc="A music Scrobbler for Last.FM radio"
arch=(x86_64)
url="http://www.last.fm/"
license=('GPL')
groups=('Multimedia')
depends=('mono' 'gstreamer0.10>=0.10.0' 'libmad' 'libgpod' 'alsa-lib' 
'gconf' 'qt')
makedepends=('deb2targz')
#checkdepends=()
#optdepends=()
#provides=()
#conflicts=()
#replaces=()
#backup=()
#options=()
install=
changelog=
source=('http://ftp.us.debian.org/debian/pool/main/l/lastfm/lastfm_1.5.4.26862+dfsg-6_amd64.deb')
#noextract=()
filename=('lastfm_1.5.4.26862+dfsg-6_amd64')
md5sums=('13eaa3a1915618f3d625f8b29fcaae14') #generate with 'makepkg -g'

build() {
  #cp $source $HOME/Downloads
  deb2targz ./$filename.deb
  #tar -xvf ./src/data.tar.gz ./src/
  
}

#check() {
 # cd "$srcdir/$pkgname-$pkgver"
 # make -k check
#}

package() {
#  cd "./src"
#  sudo pacman -U ./lastfm_1.5.4.26862+dfsg-6_amd64.tar.gz
#  make DESTDIR="$pkgdir/" install
tar -xvf ./$filename.tar.gz
sudo cp -r ./usr /
}

# vim:set ts=2 sw=2 et:
