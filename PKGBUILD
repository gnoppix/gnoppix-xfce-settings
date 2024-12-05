# Maintainer: Andreas Mueller <gnoppix@gnoppix.com>

pkgname=gnoppix-xfce-settings
pkgdesc='Gnoppix XFCE settings'
pkgver=1.0.5
pkgrel=2
arch=('any')
url="https://github.com/gnoppix/$pkgname"
license=('GPL')
makedepends=('coreutils')
source=("$pkgname-$pkgver.tar.gz::$url/archive/$pkgver.tar.gz")
sha512sums=('a106a3e6018a5b06f55443d8393ea66ccaa192fcb36ec7b10fbf6a2b3606245a2f0fb57c926ab1aa30a9daa58a19689f4a2a4de120f587188871511918320339')
depends=('gnoppix-zsh-config'
         'nerd-fonts-fantasque-sans-mono'
         'noto-fonts'
         'ttf-fira-sans'
         'kvantum-qt5'
         'qt5ct'
         'xfce4-whiskermenu-plugin'
         'thunar'
         'char-white'
         'qogir-icon-theme'
         'capitaine-cursors'
         'gnoppix-wallpapers'
         'kvantum-theme-nordic-git'
         'gnoppix-nord-gtk-theme-git')
install=$pkgname.install
provides=('gnoppix-desktop-settings')
conflicts=('gnoppix-desktop-settings')

package() {
    install -d $pkgdir/etc
    cp -rf $srcdir/$pkgname-$pkgver/etc $pkgdir
    install -d $pkgdir/usr
    cp -rf $srcdir/$pkgname-$pkgver/usr $pkgdir
}
