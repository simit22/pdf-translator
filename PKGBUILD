# Maintainer: Your Name <your_email@example.com>
pkgname=pdf-Translator
pkgver=1.0
pkgrel=1
pkgdesc="this script will translate your pdf , and create a new translated PDF  "
arch=('any')
url="https://github.com/simit22/pdf-translator"
license=('GPL')
depends=('python' 'python-pypdf2' 'python-reportlab' 'translate-shell')  # Add any other dependencies here
source=("https://github.com/simit22/pdf-translator/archive/v${pkgver}.tar.gz")

md5sums=('SKIP')  # You can generate the checksum using `makepkg -g`

package() {
    cd "${srcdir}/pdf-text-translator-${pkgver}"
    
    # Install script
    install -Dm755 pdf_text_extractor.py "${pkgdir}/usr/bin/pdf_text_extractor.py"
    
    # Install license
    install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
