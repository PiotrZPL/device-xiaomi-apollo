# Reference: <https://postmarketos.org/devicepkg>
pkgname=device-xiaomi-apollo
pkgdesc="Xiaomi Mi 10T 5G"
pkgver=0.1
pkgrel=0
url="https://postmarketos.org"
license="MIT"
arch="aarch64"
options="!check !archcheck"
#depends="
#	linux-xiaomi-apollo
#	mkbootimg
#	postmarketos-base
#"

install="$pkgname.post-install $pkgname.post-upgrade"

#depends="
#	alsa-ucm-conf-qcom-sm8250
#	make-dynpart-mappings
#	mesa-vulkan-freedreno
#	mkbootimg
#	postmarketos-base
#	postmarketos-update-kernel
#	qbootctl
#	swclock-offset
#	linux-postmarketos-qcom-sm8250
#"

depends="
	mkbootimg
	postmarketos-base
	linux-postmarketos-qcom-sm8250
	swclock-offset
	qbootctl
	postmarketos-update-kernel
	mesa-vulkan-freedreno
	make-dynpart-mappings
"

makedepends="devicepkg-dev"
source="deviceinfo"

build() {
	devicepkg_build $startdir $pkgname
}

package() {
	devicepkg_package $startdir $pkgname
}

sha512sums="
538456b4c3e449bdc7247c9f669ba2a7f14cb8d9650beedc10d480ae74ce6e2bd044328bd494aa588054951fb6044d70796adae8b700634c7af7e477c74924ac  deviceinfo
"
