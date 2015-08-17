# Maintainer: Thomas Dziedzic < gostrc at gmail >

pkgname=python2-milk
pkgver=0.4.2
pkgrel=1
pkgdesc='A machine learning toolkit with a focus on supervised classification with several classifiers.'
arch=('i686' 'x86_64')
url='http://luispedro.org/software/milk'
license=('MIT')
depends=('python2-numpy')
makedepends=('python2-distribute')
source=("http://pypi.python.org/packages/source/m/milk/milk-${pkgver}.tar.gz")
md5sums=('f4b9489ac550b5b32fb5810422b438f1')

build() {
  cd milk-${pkgver}

  python2 setup.py build
}

package() {
  cd milk-${pkgver}

  python2 setup.py install --root=${pkgdir} --optimize=1
}
