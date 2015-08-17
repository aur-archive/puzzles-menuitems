# Contributor: Graham Rogers <rogers3.14 at gmail dot com>
# Contributor: Dany Martineau <dany.luc.martineau at gmail dot com>
# Contributor: TastyPi (AUR)
# Maintainer: SanskritFritz (gmail)

pkgname=puzzles-menuitems
_menuforpkgname=puzzles
_buildver=bd0a357
pkgver=20150118
_fileversion=$pkgver.$_buildver
pkgrel=1
pkgdesc="Menu items for Simon Tatham's Portable Puzzle Collection."
arch=('any')
url="http://www.chiark.greenend.org.uk/~sgtatham/puzzles/"
license=('MIT')
#depends=("puzzles=$pkgver")
depends=("puzzles")
source=(puzzles-blackbox.desktop
        puzzles-bridges.desktop
        puzzles-cube.desktop
        puzzles-dominosa.desktop
        puzzles-fifteen.desktop
        puzzles-filling.desktop
        puzzles-flip.desktop
        puzzles-galaxies.desktop
        puzzles-guess.desktop
        puzzles-inertia.desktop
        puzzles-keen.desktop
        puzzles-lightup.desktop
        puzzles-loopy.desktop
        puzzles-magnets.desktop
        puzzles-map.desktop
        puzzles-mines.desktop
        puzzles-net.desktop
        puzzles-netslide.desktop
        puzzles-pattern.desktop
        puzzles-pearl.desktop
        puzzles-pegs.desktop
        puzzles-range.desktop
        puzzles-rect.desktop
        puzzles-samegame.desktop
        puzzles-signpost.desktop
        puzzles-singles.desktop
        puzzles-sixteen.desktop
        puzzles-slant.desktop
        puzzles-solo.desktop
        puzzles-tents.desktop
        puzzles-towers.desktop
        puzzles-twiddle.desktop
        puzzles-undead.desktop
        puzzles-unequal.desktop
	puzzles-unruly.desktop
        puzzles-untangle.desktop
        "http://www.chiark.greenend.org.uk/~sgtatham/${_menuforpkgname}/${_menuforpkgname}-${_fileversion}.tar.gz")
#	"http://www.chiark.greenend.org.uk/~sgtatham/puzzles/puzzles.tar.gz")

package() {
  install -d "${pkgdir}"/usr/share/{applications,icons/hicolor/{16x16/apps,32x32/apps,48x48/apps,352x352/apps},licenses/${pkgname}}

  cd "${srcdir}"

  install -Dm644 *.desktop "${pkgdir}/usr/share/applications/"

  cd "${srcdir}/${_menuforpkgname}-${_fileversion}"

  install -Dm644 LICENCE "${pkgdir}/usr/share/licenses/${pkgname}/"

  cd "${srcdir}/${_menuforpkgname}-${_fileversion}/icons"

  for s in 16 32 48; do
    for file in *-${s}d24.png; do
      mv ${file} "${pkgdir}/usr/share/icons/hicolor/${s}x${s}/apps/puzzles-${file%-${s}d24.png}.png"
    done
  done

  for file in *-base.png; do
    mv ${file} "${pkgdir}/usr/share/icons/hicolor/352x352/apps/puzzles-${file%-base.png}.png"
  done
}

# updpkgsums
md5sums=('30be7a4f96a9d1c728d43259c119a5b6'
         'ac9646356de9887518e70dc32f5ed2d0'
         'd3fc1ed68c945a6dde218ed7d40c1316'
         '65bd759f07e196da07cffba96fb88cc5'
         'f76ef39c7876fec7c3063e60bf5b9ed8'
         '629791d7eac932138c4edc5fc85dc231'
         'a74f0e05c5c97726385f9ecf46b2bc3d'
         'abb0352586b4d581545c44e823a4f020'
         'e5de7bc557e4737b4c98ddd1d00789c4'
         '0f44ef3aae6279eaa36f1c3b3eaa559c'
         '9ce8a7a3258b1bd7c4dbda89fa0090f8'
         '9daf81b82e4e2414282b23f259aa4ff2'
         'ab882e005e2ac0e3c4db145c021033c2'
         'c77647a97984e36b22bd81946ea16119'
         'f134407febbec0719ccb69b1ff1a4531'
         'c4281aa963fb4ca6328a9c9b7fd96530'
         'ceb06fa2829b0b5223a14fd49cd33205'
         'd6d79f2b01083ccdf9d3494b71629c35'
         '2b87f00cbbc4419013514c7a9c4cfa2f'
         '7e84578b932338e5c8948538fd79f17a'
         '68370bd171b98671d7080de9abf66ddf'
         '12d80c2952c47455ea204973631bcd02'
         '0cd8e0ae55eb2eab8a0efe9ea2424ce1'
         'e7816825f6ff042d7ab49172bb101c6d'
         '4a46fc29e3b8c5ae31f069417c0cff53'
         '83ae809e9f1f56a84538674e7f0b4c5a'
         '3d88a52fa19b093be89e18a831a3a297'
         '8e0e2a6bc69e93979233e853d7aa5c7c'
         'df12b42b1c02e3d90b7bb354efe8f85a'
         '3fa749247894083a008c47a6588225b5'
         '6bf64040158db4bf3fddde7625c79d79'
         '4c26908e23d652623c41729bc9018d74'
         '9533c961bc6342b791553abb528a9f3a'
         'df078c397e8653f6df11eac4b14a26de'
         'ed603cd73838bbbadd2f55beb444d5d8'
         'a39674ef749b092d481613483bca6d3e'
         '5f130f4e59c294abd9d29d086f5795f8')
