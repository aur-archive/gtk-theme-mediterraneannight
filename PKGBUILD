# Maintainer: grimi <grimi at poczta dot fm>

pkgname=gtk-theme-mediterraneannight
pkgver=1.15
pkgrel=1
pkgdesc="A gtk3, gtk2, metacity and unity theme (variation of 'Adwaita cupertino')."
arch=('any')
url="http://gnome-look.org/content/show.php/MediterraneanNight?content=148398"
license=('GPL')
depends=('gtk-engines' 'gtk-engine-murrine' 'gtk-engine-unico')
provides=('mediterraneannight-theme')
conflicts=('mediterraneannight-theme')
source=("${pkgname}-${pkgver}.tar.gz::http://gnome-look.org/CONTENT/content-files/148398-MediterraneanNight.tar.gz")
md5sums=('24e12ba8d301edbdb44f6a85159b6782')


package() {
  # delete custom buttons for metacity and unity
  rm MediterraneanNight/*.tar.gz

  find Mediterranean{Light,Night,Dark}/ -type f \
      -exec install -Dm644 "{}" "$pkgdir/usr/share/themes/{}" \;
}

# vim:set ts=2 sw=2 et:
