pkgname=maketxt
pkgver=1.0.0
pkgrel=1
pkgdesc="maketxt is a simple cli tool that creates .txt files."
arch=('any')
url="https://github.com/skirexwastaken/maketxt"
license=('MIT')
depends=('python')
makedepends=('python-setuptools')

source=("maketxt.py"
        "setup.py")
sha256sums=('SKIP'
            'SKIP')

build() {
    cd "$srcdir"
    python setup.py build
}

package() {
    cd "$srcdir"
    python setup.py install --root="$pkgdir" --optimize=1 --skip-build
}
