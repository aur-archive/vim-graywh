# Maintainer: Laszlo Papp <djszapi @ gmail at com>
pkgname=vim-graywh
pkgver=1
_scriptid=10438
pkgrel=1
pkgdesc="My personal colorscheme"
arch=(i686 x86_64)
url="http://www.vim.org/scripts/script.php?script_id=2616"
license=('custom')
depends=(vim)
groups=('vim-plugins')
install=vimdoc.install
source=(${pkgname}::http://www.vim.org/scripts/download_script.php?src_id=${_scriptid}
        license.txt)
md5sums=('9e869b691fd99ea590339271446cc85a'
         'efbd5986e691ce8c876fb86e8f5961ea')

build() {
    install -Dm755 ${srcdir}/${pkgname} ${pkgdir}/usr/share/vim/colors/graywh.vim || return 1
    install -Dm755 ${srcdir}/license.txt ${pkgdir}/usr/share/licenses/${pkgname}/license.txt
}
