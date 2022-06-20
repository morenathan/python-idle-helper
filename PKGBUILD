# Maintainer: Nathan Middleton <nathan@aplace.us>
pkgname=python-idle-helper
pkgver=1
pkgrel=1
pkgdesc="XDG Desktop fiels and mime assocations for Python IDLE IDE."
arch=('any')
url="https://github.com/morenathan/python-idle-helper"
install="install"
license=('GPL2')
groups=('nm' 
		'python')
depends=('python'
		 'shared-mime-info')
source=("application-x-idle.xml"
		"org.python.idle.desktop"
		"LICENSE")
sha256sums=('c876afda4066bfef2424785afbe99b89fca8304bcff2568a685f3da5e96a3a0d'
            '83c2001e85c5069707122ca2686c3b86e24a9ae733b6bc67d53a64f138a7a0d8'
            '9deb227fe7735b67c0fb33153e2c707c57bab378d0fbedd1d82d75e418eba9cf')

package() {
	install -Dm644 "application-x-idle.xml" "${pkgdir}/usr/share/mime/packages/application-x-idle.xml"
	install -Dm644 "org.python.idle.desktop" "${pkgdir}/usr/share/applications/org.python.idle.desktop"
	install -Dm644 "LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
