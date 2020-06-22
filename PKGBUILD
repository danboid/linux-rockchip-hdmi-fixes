# AArch64 multi-platform
# Contributor: Kevin Mihelich <kevin@archlinuxarm.org>
# Maintainer: Dan Johansen <strit@manjaro.org>

pkgbase=linux-aarch64
_srcname=linux-5.7
_kernelname=${pkgbase#linux}
_desc="AArch64 multi-platform"
pkgver=5.7.5
pkgrel=1
arch=('aarch64')
url="http://www.kernel.org/"
license=('GPL2')
makedepends=('xmlto' 'docbook-xsl' 'kmod' 'inetutils' 'bc' 'git' 'uboot-tools' 'dtc')
options=('!strip')
source=("http://www.kernel.org/pub/linux/kernel/v5.x/${_srcname}.tar.xz"
        "http://www.kernel.org/pub/linux/kernel/v5.x/patch-${pkgver}.xz"
        '0001-net-smsc95xx-Allow-mac-address-to-be-set-as-a-parame.patch'
        '0003-arm64-dts-rockchip-add-usb3-controller-node-for-RK33.patch'
        '0004-arm64-dts-rockchip-enable-usb3-nodes-on-rk3328-rock6.patch'
        '0001-arm64-dts-rockchip-add-pcie-node-rockpi4.patch'
        '0002-arm64-dts-rockchip-modify-pcie-node-rockpro64.patch'
        '0003-text_offset.patch'
        '0004-board-rockpi4-dts-upper-port-host.patch'
        '0005-dt-bindings-arm-amlogic-add-odroid-c4-bindings.patch'
        '0006-arm64-dts-meson-sm1-add-support-for-Hardkernel-ODROID-C4.patch'
        '0007-arm64-dts-rockchip-add-HDMI-sound-node-for-rk3328-ro.patch'
        '0008-arm64-dts-allwinner-add-hdmi-sound-to-pine-devices.patch'
        '0009-drivers-power-supply-Add-support-for-cw2015.patch'
        '0010-arm64-dts-rockchip-add-cw2015-node-to-PBP.patch'
        '0011-fix-wonky-wifi-bt-on-PBP.patch'
        '0012-add-suspend-to-rk3399-PBP.patch'
        '0013-arm64-dts-rockchip-setup-USB-type-c-port-as-dual-dat.patch'
        '0014-arm64-dts-rockchip-fix-roc-cc-dts.patch'
        '0015-add-dp-alt-mode-to-PBP.patch'
        '0016-arm64-dts-allwinner-add-ohci-ehci-to-h5-nanopi.patch'
        '0001-Bluetooth-Add-new-quirk-for-broken-local-ext-features-max_page.patch'
        '0002-Bluetooth-hci_h5-Add-support-for-reset-GPIO.patch'
        '0003-dt-bindings-net-bluetooth-Add-rtl8723bs-bluetooth.patch'
        '0004-Bluetooth-hci_h5-Add-support-for-binding-RTL8723BS-with-device-tree.patch'
        '0005-Bluetooth-btrtl-add-support-for-the-RTL8723CS.patch'
        '0006-bluetooth-btrtl-Make-more-space-for-config-firmware-file-name.patch'
        '0007-arm64-dts-allwinner-add-bluetooth-to-pinebook.patch'
        '0008-drm-sun8i-ui-vi-Fix-layer-zpos-change-atomic-modesetting.patch'
        '0009-drm-sun4i-Mark-one-of-the-UI-planes-as-a-cursor-one.patch'
        '0010-drm-sun4i-drm-Recover-from-occasional-HW-failures.patch'
        '0011-arm64-dts-allwinner-enable-bluetooth-pinetab-pinepho.patch'
        'config'
        'linux.preset'
        '60-linux.hook'
        '90-linux.hook'
        '0001-bootsplash.patch'
        '0002-bootsplash.patch'
        '0003-bootsplash.patch'
        '0004-bootsplash.patch'
        '0005-bootsplash.patch'
        '0006-bootsplash.patch'
        '0007-bootsplash.patch'
        '0008-bootsplash.patch'
        '0009-bootsplash.patch'
        '0010-bootsplash.patch'
        '0011-bootsplash.patch'
        '0012-bootsplash.patch')
md5sums=('f63ed18935914e1ee3e04c2a0ce1ba3b'
         '7c8a48752659cb86ceb904d8f1117c76'
         '6ee347975dca719ecd63a846cc5983b2'
         '9986e28b5c2c3c62a5c3bb53abd94640'
         '552ea82c3a5e14ca9149da8c4b4d5a82'
         '7b6f548fc352a4c530eae58f6a69041f'
         '39fc489449d519b45532631825840f3d'
         'fd5919b02b1dd17f62dd51d57986368f'
         'f7769084356056b5eec725938e49a6a5'
         '48143f15b156bb4235b0cd2880ada128'
         '998c32f4db54cc9460c967029612a420'
         '345e1329e2b6a530554d8538415caebe'
         'fa586447846ec5aef8ab972058c5548e'
         'd235bd43604bba10d878e066d80846ef'
         '7ca26d7c90227224769e176043dd7fa9'
         'ad3ba520c225abe8be59f271a4a23dc1'
         '1ac243c06d58a2e6fe23e9934a9fcbcb'
         '4993c45194869f54a187942cb04dea0e'
         '4945a41035d9054924e207a0f40420e4'
         'fa88f0acd760bae15f8ae71518cea8b3'
         'e6fe272dc95a1c0a8f871924699fea16'
         '762937f4765b5c22f58d3a4a3c4cfd46'
         'f70bc0e4a81a05f6de3e8ef8c31233c4'
         '5a0aea477134c1851d6ef4ed395e044a'
         'b35ee0bf7b5b0282c1f24c7bc0a690ad'
         'aaa12633b3bcfdd223ea939690aa7c2d'
         'e1285a487f967f0594a098fcba708cac'
         '2fad5ce2eaa1786b4217c575add0af8f'
         '929f2d20a44be5b5d7c6a5134c660a79'
         '22c651017f864e41916a74e63ef46a19'
         'bf9f906cca7b7489d3123a249dcbd021'
         'a74fcfa1e085a3a99dcf4f214c1ca65a'
         '50ba501efc4cdbb9d5b16b560243ac1e'
         '86d4a35722b5410e3b29fc92dae15d4b'
         'ce6c81ad1ad1f8b333fd6077d47abdaf'
         '3dc88030a8f2f5a5f97266d99b149f77'
         'f13cfcd8a4667ecca68bccefee4b8283'
         'b4acd66a564af83b5409738c40b4a566'
         'a6407dceae1838f5aa27450401a91be6'
         'cb78b1c11b917a4d31c4b1567183b76f'
         '3efea575da7f02ba94789d3b6b81e11f'
         '2529ad13791b259d80c9d5d702187a65'
         'efd2367798cc4eab0e15fc0ae44fb003'
         '50255aac36e002afa477e4527a0550af'
         '6b6def41b404422dc04b39e2f1adffc8'
         '1922e3a7727d2bf51641b98d6d354738'
         'd6b7e4e43e42128cf950251e0d0aee23'
         'ecfd8a30c480149005fcf349e4d06f4b')

prepare() {
  cd ${_srcname}

  # add upstream patch
  patch -Np1 -i "${srcdir}/patch-${pkgver}"

  # ALARM patches
  patch -Np1 -i "${srcdir}/0001-net-smsc95xx-Allow-mac-address-to-be-set-as-a-parame.patch"     #All
  patch -Np1 -i "${srcdir}/0003-arm64-dts-rockchip-add-usb3-controller-node-for-RK33.patch"     #RK3328
  patch -Np1 -i "${srcdir}/0004-arm64-dts-rockchip-enable-usb3-nodes-on-rk3328-rock6.patch"     #RK3328
  
  # Manjaro ARM Patches
  patch -Np1 -i "${srcdir}/0001-arm64-dts-rockchip-add-pcie-node-rockpi4.patch"                 #Rock Pi 4
  patch -Np1 -i "${srcdir}/0002-arm64-dts-rockchip-modify-pcie-node-rockpro64.patch"            #RockPro64
  patch -Np1 -i "${srcdir}/0003-text_offset.patch"                                              #Amlogic
  patch -Np1 -i "${srcdir}/0004-board-rockpi4-dts-upper-port-host.patch"                        #Rock Pi 4
  patch -Np1 -i "${srcdir}/0005-dt-bindings-arm-amlogic-add-odroid-c4-bindings.patch"           #Odroid C4 (added in 5.8)
  patch -Np1 -i "${srcdir}/0006-arm64-dts-meson-sm1-add-support-for-Hardkernel-ODROID-C4.patch" #Odroid C4 (added in 5.8)
  patch -Np1 -i "${srcdir}/0007-arm64-dts-rockchip-add-HDMI-sound-node-for-rk3328-ro.patch"     #Rock64
  patch -Np1 -i "${srcdir}/0008-arm64-dts-allwinner-add-hdmi-sound-to-pine-devices.patch"       #Pine64
  patch -Np1 -i "${srcdir}/0009-drivers-power-supply-Add-support-for-cw2015.patch"              #Pinebook Pro (added in 5.8)
  patch -Np1 -i "${srcdir}/0010-arm64-dts-rockchip-add-cw2015-node-to-PBP.patch"                #Pinebook Pro
  patch -Np1 -i "${srcdir}/0011-fix-wonky-wifi-bt-on-PBP.patch"                                 #Pinebook Pro
  patch -Np1 -i "${srcdir}/0012-add-suspend-to-rk3399-PBP.patch"                                #Pinebook Pro
  patch -Np1 -i "${srcdir}/0013-arm64-dts-rockchip-setup-USB-type-c-port-as-dual-dat.patch"     #Pinebook Pro
  patch -Np1 -i "${srcdir}/0014-arm64-dts-rockchip-fix-roc-cc-dts.patch"                        #Roc-CC
  patch -Np1 -i "${srcdir}/0015-add-dp-alt-mode-to-PBP.patch"                                   #Pinebook Pro
  patch -Np1 -i "${srcdir}/0016-arm64-dts-allwinner-add-ohci-ehci-to-h5-nanopi.patch"           #Nanopi Neo Plus 2
  
  # Pinebook patches
  patch -Np1 -i "${srcdir}/0001-Bluetooth-Add-new-quirk-for-broken-local-ext-features-max_page.patch"
  patch -Np1 -i "${srcdir}/0002-Bluetooth-hci_h5-Add-support-for-reset-GPIO.patch"
  patch -Np1 -i "${srcdir}/0003-dt-bindings-net-bluetooth-Add-rtl8723bs-bluetooth.patch"
  patch -Np1 -i "${srcdir}/0004-Bluetooth-hci_h5-Add-support-for-binding-RTL8723BS-with-device-tree.patch"
  patch -Np1 -i "${srcdir}/0005-Bluetooth-btrtl-add-support-for-the-RTL8723CS.patch"
  patch -Np1 -i "${srcdir}/0006-bluetooth-btrtl-Make-more-space-for-config-firmware-file-name.patch"
  patch -Np1 -i "${srcdir}/0007-arm64-dts-allwinner-add-bluetooth-to-pinebook.patch"
  patch -Np1 -i "${srcdir}/0008-drm-sun8i-ui-vi-Fix-layer-zpos-change-atomic-modesetting.patch"
  patch -Np1 -i "${srcdir}/0009-drm-sun4i-Mark-one-of-the-UI-planes-as-a-cursor-one.patch"
  patch -Np1 -i "${srcdir}/0010-drm-sun4i-drm-Recover-from-occasional-HW-failures.patch"
  patch -Np1 -i "${srcdir}/0011-arm64-dts-allwinner-enable-bluetooth-pinetab-pinepho.patch"
  
  # Bootsplash patches
  patch -Np1 -i "${srcdir}/0001-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0002-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0003-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0004-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0005-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0006-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0007-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0008-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0009-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0010-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0011-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0012-bootsplash.patch"
  
  cat "${srcdir}/config" > ./.config

  # add pkgrel to extraversion
  sed -ri "s|^(EXTRAVERSION =)(.*)|\1 \2-${pkgrel}|" Makefile

  # don't run depmod on 'make install'. We'll do this ourselves in packaging
  sed -i '2iexit 0' scripts/depmod.sh
}

build() {
  cd ${_srcname}

  # get kernel version
  make prepare

  # load configuration
  # Configure the kernel. Replace the line below with one of your choice.
  #make menuconfig # CLI menu for configuration
  #make nconfig # new CLI menu for configuration
  #make xconfig # X-based configuration
  #make oldconfig # using old config from previous kernel version
  # ... or manually edit .config

  # Copy back our configuration (use with new kernel version)
  #cp ./.config /var/tmp/${pkgbase}.config

  ####################
  # stop here
  # this is useful to configure the kernel
  #msg "Stopping build"
  #return 1
  ####################

  #yes "" | make config

  # build!
  unset LDFLAGS
  make ${MAKEFLAGS} Image Image.gz modules
  # Generate device tree blobs with symbols to support applying device tree overlays in U-Boot
  make ${MAKEFLAGS} DTC_FLAGS="-@" dtbs
}

_package() {
  pkgdesc="The Linux Kernel and modules - ${_desc}"
  depends=('coreutils' 'linux-firmware' 'kmod' 'mkinitcpio>=0.7')
  optdepends=('crda: to set the correct wireless channels of your country')
  provides=('kernel26' "linux=${pkgver}")
  replaces=('linux-armv8')
  conflicts=('linux')
  backup=("etc/mkinitcpio.d/${pkgbase}.preset")
  install=${pkgname}.install

  cd ${_srcname}

  KARCH=arm64

  # get kernel version
  _kernver="$(make kernelrelease)"
  _basekernel=${_kernver%%-*}
  _basekernel=${_basekernel%.*}

  mkdir -p "${pkgdir}"/{boot,usr/lib/modules}
  make INSTALL_MOD_PATH="${pkgdir}/usr" modules_install
  make INSTALL_DTBS_PATH="${pkgdir}/boot/dtbs" dtbs_install
  cp arch/$KARCH/boot/Image{,.gz} "${pkgdir}/boot"

  # make room for external modules
  local _extramodules="extramodules-${_basekernel}${_kernelname}"
  ln -s "../${_extramodules}" "${pkgdir}/usr/lib/modules/${_kernver}/extramodules"

  # add real version for building modules and running depmod from hook
  echo "${_kernver}" |
    install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_extramodules}/version"

  # remove build and source links
  rm "${pkgdir}"/usr/lib/modules/${_kernver}/{source,build}

  # now we call depmod...
  depmod -b "${pkgdir}/usr" -F System.map "${_kernver}"

  # add vmlinux
  install -Dt "${pkgdir}/usr/lib/modules/${_kernver}/build" -m644 vmlinux

  # sed expression for following substitutions
  local _subst="
    s|%PKGBASE%|${pkgbase}|g
    s|%KERNVER%|${_kernver}|g
    s|%EXTRAMODULES%|${_extramodules}|g
  "

  # install mkinitcpio preset file
  sed "${_subst}" ../linux.preset |
    install -Dm644 /dev/stdin "${pkgdir}/etc/mkinitcpio.d/${pkgbase}.preset"

  # install pacman hooks
  sed "${_subst}" ../60-linux.hook |
    install -Dm644 /dev/stdin "${pkgdir}/usr/share/libalpm/hooks/60-${pkgbase}.hook"
  sed "${_subst}" ../90-linux.hook |
    install -Dm644 /dev/stdin "${pkgdir}/usr/share/libalpm/hooks/90-${pkgbase}.hook"
}

_package-headers() {
  pkgdesc="Header files and scripts for building modules for linux kernel - ${_desc}"
  provides=("linux-headers=${pkgver}")
  conflicts=('linux-headers')

  cd ${_srcname}
  local _builddir="${pkgdir}/usr/lib/modules/${_kernver}/build"

  install -Dt "${_builddir}" -m644 Makefile .config Module.symvers
  install -Dt "${_builddir}/kernel" -m644 kernel/Makefile

  mkdir "${_builddir}/.tmp_versions"

  cp -t "${_builddir}" -a include scripts

  install -Dt "${_builddir}/arch/${KARCH}" -m644 arch/${KARCH}/Makefile
  install -Dt "${_builddir}/arch/${KARCH}/kernel" -m644 arch/${KARCH}/kernel/asm-offsets.s arch/$KARCH/kernel/module.lds

  cp -t "${_builddir}/arch/${KARCH}" -a arch/${KARCH}/include
  mkdir -p "${_builddir}/arch/arm"
  cp -t "${_builddir}/arch/arm" -a arch/arm/include

  install -Dt "${_builddir}/drivers/md" -m644 drivers/md/*.h
  install -Dt "${_builddir}/net/mac80211" -m644 net/mac80211/*.h

  # http://bugs.archlinux.org/task/13146
  install -Dt "${_builddir}/drivers/media/i2c" -m644 drivers/media/i2c/msp3400-driver.h

  # http://bugs.archlinux.org/task/20402
  install -Dt "${_builddir}/drivers/media/usb/dvb-usb" -m644 drivers/media/usb/dvb-usb/*.h
  install -Dt "${_builddir}/drivers/media/dvb-frontends" -m644 drivers/media/dvb-frontends/*.h
  install -Dt "${_builddir}/drivers/media/tuners" -m644 drivers/media/tuners/*.h

  # add xfs and shmem for aufs building
  mkdir -p "${_builddir}"/{fs/xfs,mm}

  # copy in Kconfig files
  find . -name Kconfig\* -exec install -Dm644 {} "${_builddir}/{}" \;

  # remove unneeded architectures
  local _arch
  for _arch in "${_builddir}"/arch/*/; do
    [[ ${_arch} == */${KARCH}/ || ${_arch} == */arm/ ]] && continue
    rm -r "${_arch}"
  done

  # remove files already in linux-docs package
  rm -r "${_builddir}/Documentation"

  # remove now broken symlinks
  find -L "${_builddir}" -type l -printf 'Removing %P\n' -delete

  # Fix permissions
  chmod -R u=rwX,go=rX "${_builddir}"

  # strip scripts directory
  local _binary _strip
  while read -rd '' _binary; do
    case "$(file -bi "${_binary}")" in
      *application/x-sharedlib*)  _strip="${STRIP_SHARED}"   ;; # Libraries (.so)
      *application/x-archive*)    _strip="${STRIP_STATIC}"   ;; # Libraries (.a)
      *application/x-executable*) _strip="${STRIP_BINARIES}" ;; # Binaries
      *) continue ;;
    esac
    /usr/bin/strip ${_strip} "${_binary}"
  done < <(find "${_builddir}/scripts" -type f -perm -u+w -print0 2>/dev/null)
}

pkgname=("${pkgbase}" "${pkgbase}-headers")
for _p in ${pkgname[@]}; do
  eval "package_${_p}() {
    _package${_p#${pkgbase}}
  }"
done
