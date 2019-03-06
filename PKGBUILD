# Maintainer: Andrew Kramer <andrew@jmpesp.org>
pkgname=ghidra
pkgver=9.0
pkgrel=20190228
epoch=
pkgdesc="A software reverse engineering (SRE) suite of tools developed by NSA"
arch=('any')
url="https://ghidra-sre.org/"
license=('Apache')
groups=()
depends=('jdk-openjdk>=11' 'jre-openjdk>=11')
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=(
	"https://ghidra-sre.org/${pkgname}_${pkgver}_PUBLIC_${pkgrel}.zip"
	"ghidra.desktop"
	"ghidra.png"
)
noextract=()
sha512sums=(
	'711d639da04cc7dd5b47985962cce448e5d5ea2e796e33edcc4285d119998ebab1b9403c697fa5266d8c3e834b55f79edef004a0b1741250bf584b77c92c7529'
	'0e2b7f0536f60b45ce4b4d5eaaa64db51c1fb01b074facf5561c135980a1c9f913ab1a7607fe42af1c939e27366bf2c8de37771851a0e0d8d6f7a18dadba2dcb'
	'e114d850a8092b453056f9e85cc7f94c41a62e1d4f6191d795650e06543e0686a303830a67095750d095b0ccf0e176a9b83a5e167f59429ad975bba19b497866'
)
validpgpkeys=()

#prepare() {
#}

#build() {
#}

#check() {
#}

package() {

	mkdir ${pkgdir}/opt/
	mkdir -p ${pkgdir}/usr/share/icons/hicolor/128x128/apps/
	mkdir -p ${pkgdir}/usr/share/applications/
	mkdir -p ${pkgdir}/usr/share/$pgkname/
	mkdir -p ${pkgdir}/usr/bin/
	ln -s /opt/ghidra/ghidraRun ${pkgdir}/usr/bin/ghidra

	cp -R ${srcdir}/${pkgname}_${pkgver}/ ${pkgdir}/opt/$pkgname
	cp ${srcdir}/${pkgname}.png ${pkgdir}/usr/share/icons/hicolor/128x128/apps/
	cp ${srcdir}/${pkgname}.desktop ${pkgdir}/usr/share/applications/$pkgname.desktop

}