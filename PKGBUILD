# AArch64 multi-platform
# Maintainer: Dan Johansen <strit@manjaro.org>
# Contributor: Kevin Mihelich <kevin@archlinuxarm.org>

pkgbase=linux
_srcname=linux-5.16
_kernelname=${pkgbase#linux}
_desc="AArch64 multi-platform"

pkgver=5.16.7
pkgrel=2
arch=('aarch64')
url="http://www.kernel.org/"
license=('GPL2')
makedepends=('xmlto' 'docbook-xsl' 'kmod' 'inetutils' 'bc' 'git' 'dtc')
options=('!strip')
source=("http://www.kernel.org/pub/linux/kernel/v5.x/${_srcname}.tar.xz"
        "http://www.kernel.org/pub/linux/kernel/v5.x/patch-${pkgver}.xz"
        '0001-arm64-dts-allwinner-add-hdmi-sound-to-pine-devices.patch'
        '0002-arm64-dts-allwinner-add-ohci-ehci-to-h5-nanopi.patch'
        '0003-drm-bridge-analogix_dp-Add-enable_psr-param.patch'                   # From list: https://patchwork.kernel.org/project/dri-devel/patch/20200626033023.24214-2-shawn@anastas.io/
        '0004-gpu-drm-add-new-display-resolution-2560x1440.patch'
        '0005-nuumio-panfrost-Silence-Panfrost-gem-shrinker-loggin.patch'
        '0006-arm64-dts-rockchip-Add-Firefly-Station-p1-support.patch'
        '0007-typec-displayport-some-devices-have-pin-assignments-reversed.patch'  # Not upstreamable
        '0008-Add-megis-extcon-changes-to-fusb302.patch'                           # Not upstreamable
        '0009-usb-typec-Add-megis-typex-to-extcon-bridge-driver.patch'             # Not upstreamable
        '0010-arm64-rockchip-add-DP-ALT-rockpro64.patch'                           # Not upstreamable
        '0011-ayufan-drm-rockchip-add-support-for-modeline-32MHz-e.patch'
        '0011-libreelec_rockchip_hdmi.patch' # LibreELEC HDMI fixes for rockchip
        '0012-rk3399-rp64-pcie-Reimplement-rockchip-PCIe-bus-scan-delay.patch'
        '0013-arm64-dts-rockchip-add-typec-extcon-hack.patch'                      # Not upstreamable, needs cdn_dp enabled
        '0014-drm-meson-add-YUV422-output-support.patch'
        '0015-arm64-dts-meson-add-initial-Beelink-GT1-Ultimate-dev.patch'
        '0016-add-ugoos-device.patch'
        '0017-drm-panfrost-scheduler-fix.patch'
        '0018-arm64-dts-rockchip-Add-pcie-bus-scan-delay-to-rockpr.patch'
        '0019-drm-rockchip-support-gamma-control-on-RK3399.patch'                  # From list: https://patchwork.kernel.org/project/linux-arm-kernel/cover/20211019215843.42718-1-sigmaris@gmail.com/
        '0020-media-rockchip-rga-do-proper-error-checking-in-probe.patch'          # From list: https://patchwork.kernel.org/project/linux-rockchip/patch/20211120122321.20253-1-kmcopper@danwin1210.me/
        '0021-arm-dts-rockchip-firefly-station-m2.patch'
        '0022-add-dts-rk3568-station-p2.patch'
        '0023-add-dts-rk3568-radxa-rock3a.patch'
        '0024-arm64-dts-rockchip-switch-to-hs200-on-rockpi4.patch'
        '0025-rk3399-increase-pcie-link-speed.patch'
        '0001-Bluetooth-Add-new-quirk-for-broken-local-ext-features.patch'         # From list: https://patchwork.kernel.org/project/bluetooth/patch/20200705195110.405139-2-anarsoul@gmail.com/
        '0002-Bluetooth-btrtl-add-support-for-the-RTL8723CS.patch'                 # From list: https://patchwork.kernel.org/project/bluetooth/patch/20200705195110.405139-3-anarsoul@gmail.com/
        '0003-arm64-allwinner-a64-enable-Bluetooth-On-Pinebook.patch'              # From list: https://patchwork.kernel.org/project/bluetooth/patch/20200705195110.405139-4-anarsoul@gmail.com/
        '0004-arm64-dts-allwinner-enable-bluetooth-pinetab-pinepho.patch'          # Pinephone part is in linux-next
        '0005-staging-add-rtl8723cs-driver.patch'                                  # Not upstreamable
        '0006-pinetab-accelerometer.patch'
        '0007-enable-jack-detection-pinetab.patch'
        'config'
        'linux.preset'
        '60-linux.hook'
        '90-linux.hook')
md5sums=('e6680ce7c989a3efe58b51e3f3f0bf93'
         '58ed014f8501484f3a21668c85f81327'
         '0d47dea87f03bf36262171e01889f832'
         'e6fe272dc95a1c0a8f871924699fea16'
         '9f27b2a05eaeb1995fc0fcf6a8b923c4'
         '6f592c11f6adc1de0f06e5d18f8c2862'
         'f8f0b124c741be61d86bea8d44e875f9'
         '564136ab1c75b6dc67be02b54e695ae5'
         'a033be22c23afb1d5daeeeb21353185d'
         '069797069722b8eb55eae145d13c2c6a'
         '8b73e8b7df4eeb214a93f12a0c9497c6'
         '03d78b64dd24b607b94577dca08f7cfe'
         '634a9e64dc95bb3797aacd1a64b8ee09'
         '673f9c586f9894c8a132a9a3e91c7fe2'
         '245858f26512dfc48adbf509b6fc8364'
         '4b3dc1563f1e25b34bac22c2197f2c93'
         '469417b64e6a2bf65bd74c6d9cad2040'
         '8f4816a1ed98f80eebad49b6446427a9'
         '1b92d7617e60d3c525a4b18ab4351185'
         '140b727650029bf2d99f2d176f0876d8'
         '15756f568490dcc1454b4fa4a50a9bc2'
         '19e2279811700cd8aa4ab326603d2f61'
         '72030cbfe655fc94b28ea289ee3a53a8'
         '7b23ad49405f14618cfd92f59c25b911'
         '0ef7f4e1e2e87797be664541ad33e464'
         '516a0c0f0dc663419ed275b94edbab55'
         'a0f649f78c857a01e1680b89b58b05eb'
         'ab1bda47036895103fb63063af747777'
         'cf64831f27bb47da29e708b7243bb340'
         'a100d32aa6c345290061d2a773bf1232'
         '9510821113c122f91f47b9d0f7ca7264'
         'a74fcfa1e085a3a99dcf4f214c1ca65a'
         '959c2cb33566b27f880c178039d6c12f'
         'd0fd6bd627223d4c9fc001ffff9df401'
         'f79300740a7350d2d24ab5e120831b52'
         '9d095827f8a73432ca4ed8ae50e292c5'
         '86d4a35722b5410e3b29fc92dae15d4b'
         'ce6c81ad1ad1f8b333fd6077d47abdaf'
         '3dc88030a8f2f5a5f97266d99b149f77')

prepare() {
  cd ${_srcname}

  # add upstream patch
  patch -Np1 -i "${srcdir}/patch-${pkgver}"

  # ALARM patches
  
  # Manjaro ARM Patches

  patch -Np1 -i "${srcdir}/0001-arm64-dts-allwinner-add-hdmi-sound-to-pine-devices.patch"            # Pine64
  patch -Np1 -i "${srcdir}/0002-arm64-dts-allwinner-add-ohci-ehci-to-h5-nanopi.patch"                # Nanopi Neo Plus 2
  patch -Np1 -i "${srcdir}/0003-drm-bridge-analogix_dp-Add-enable_psr-param.patch"                   # Pinebook Pro
  patch -Np1 -i "${srcdir}/0004-gpu-drm-add-new-display-resolution-2560x1440.patch"                  # Odroid
  patch -Np1 -i "${srcdir}/0005-nuumio-panfrost-Silence-Panfrost-gem-shrinker-loggin.patch"          # Panfrost
  patch -Np1 -i "${srcdir}/0006-arm64-dts-rockchip-Add-Firefly-Station-p1-support.patch"             # Firelfy Station P1
  patch -Np1 -i "${srcdir}/0007-typec-displayport-some-devices-have-pin-assignments-reversed.patch"  # DP Alt Mode
  patch -Np1 -i "${srcdir}/0008-Add-megis-extcon-changes-to-fusb302.patch"                           # DP Alt Mode
  patch -Np1 -i "${srcdir}/0009-usb-typec-Add-megis-typex-to-extcon-bridge-driver.patch"             # DP Alt Mode
  patch -Np1 -i "${srcdir}/0010-arm64-rockchip-add-DP-ALT-rockpro64.patch"                           # DP Alt mode - RockPro64
  patch -Np1 -i "${srcdir}/0011-ayufan-drm-rockchip-add-support-for-modeline-32MHz-e.patch"          # DP Alt mode
  patch -Np1 -i "${srcdir}/0011-libreelec_rockchip_hdmi.patch"                                          #HDMI LibreELEC - RK3399/RK3328
  patch -Np1 -i "${srcdir}/0012-rk3399-rp64-pcie-Reimplement-rockchip-PCIe-bus-scan-delay.patch"     # RockPro64
  patch -Np1 -i "${srcdir}/0013-arm64-dts-rockchip-add-typec-extcon-hack.patch"                      # DP Alt mode
  patch -Np1 -i "${srcdir}/0014-drm-meson-add-YUV422-output-support.patch"                           # G12B
  patch -Np1 -i "${srcdir}/0015-arm64-dts-meson-add-initial-Beelink-GT1-Ultimate-dev.patch"          # Beelink
  patch -Np1 -i "${srcdir}/0016-add-ugoos-device.patch"                                              # Ugoos
  patch -Np1 -i "${srcdir}/0017-drm-panfrost-scheduler-fix.patch"                                    # Panfrost
  patch -Np1 -i "${srcdir}/0018-arm64-dts-rockchip-Add-pcie-bus-scan-delay-to-rockpr.patch"          # RockPro64
  patch -Np1 -i "${srcdir}/0019-drm-rockchip-support-gamma-control-on-RK3399.patch"                  # RK3399
  patch -Np1 -i "${srcdir}/0020-media-rockchip-rga-do-proper-error-checking-in-probe.patch"          # Rockchip
  #patch -Np1 -i "${srcdir}/0021-arm-dts-rockchip-firefly-station-m2.patch"                          # Firefly Station M2
  #patch -Np1 -i "${srcdir}/0022-add-dts-rk3568-station-p2.patch"                                    # Firefly Station P2
  #patch -Np1 -i "${srcdir}/0023-add-dts-rk3568-radxa-rock3a.patch"                                  # Radxa Rock3A
  patch -Np1 -i "${srcdir}/0024-arm64-dts-rockchip-switch-to-hs200-on-rockpi4.patch"                 # Rock Pi 4
  patch -Np1 -i "${srcdir}/0025-rk3399-increase-pcie-link-speed.patch"                               # RK3399

  # Pinebook, PinePhone and PineTab patches
  patch -Np1 -i "${srcdir}/0001-Bluetooth-Add-new-quirk-for-broken-local-ext-features.patch"         # Bluetooth
  patch -Np1 -i "${srcdir}/0002-Bluetooth-btrtl-add-support-for-the-RTL8723CS.patch"                 # Bluetooth
  patch -Np1 -i "${srcdir}/0003-arm64-allwinner-a64-enable-Bluetooth-On-Pinebook.patch"              # Bluetooth
  patch -Np1 -i "${srcdir}/0004-arm64-dts-allwinner-enable-bluetooth-pinetab-pinepho.patch"          # Bluetooth
  patch -Np1 -i "${srcdir}/0005-staging-add-rtl8723cs-driver.patch"                                  # Wifi
  patch -Np1 -i "${srcdir}/0006-pinetab-accelerometer.patch"                                         # Accelerometer
  patch -Np1 -i "${srcdir}/0007-enable-jack-detection-pinetab.patch"                                 # Audio
  
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
  make ${MAKEFLAGS} Image modules
  # Generate device tree blobs with symbols to support applying device tree overlays in U-Boot
  make ${MAKEFLAGS} DTC_FLAGS="-@" dtbs
}

_package() {
  pkgdesc="The Linux Kernel and modules - ${_desc}"
  depends=('coreutils' 'linux-firmware' 'kmod' 'initramfs')
  optdepends=('crda: to set the correct wireless channels of your country')
  provides=('kernel26' "linux=${pkgver}")
  conflicts=('kernel26' 'linux')
  replaces=('linux-armv8' 'linux-aarch64')
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
  cp arch/$KARCH/boot/Image "${pkgdir}/boot"

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
  replaces=('linux-aarch64-headers')

  cd ${_srcname}
  local _builddir="${pkgdir}/usr/lib/modules/${_kernver}/build"

  install -Dt "${_builddir}" -m644 Makefile .config Module.symvers
  install -Dt "${_builddir}/kernel" -m644 kernel/Makefile

  mkdir "${_builddir}/.tmp_versions"

  cp -t "${_builddir}" -a include scripts

  install -Dt "${_builddir}/arch/${KARCH}" -m644 arch/${KARCH}/Makefile
  install -Dt "${_builddir}/arch/${KARCH}/kernel" -m644 arch/${KARCH}/kernel/asm-offsets.s
  install -Dt "${_builddir}" -m644 vmlinux 

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

  # remove documentation files
  rm -r "${_builddir}/Documentation"

  # remove now broken symlinks
  find -L "${_builddir}" -type l -printf 'Removing %P\n' -delete

  # strip scripts directory
  local file
  while read -rd '' file; do
    case "$(file -bi "$file")" in
      application/x-sharedlib\;*)      # Libraries (.so)
        strip $STRIP_SHARED "$file" ;;
      application/x-archive\;*)        # Libraries (.a)
        strip $STRIP_STATIC "$file" ;;
      application/x-executable\;*)     # Binaries
        strip $STRIP_BINARIES "$file" ;;
      application/x-pie-executable\;*) # Relocatable binaries
        strip $STRIP_SHARED "$file" ;;
    esac
  done < <(find "${_builddir}" -type f -perm -u+x ! -name vmlinux -print0 2>/dev/null)
  strip $STRIP_STATIC "${_builddir}/vmlinux"
  
  # remove unwanted files
  find ${_builddir} -name '*.orig' -delete
}

pkgname=("${pkgbase}" "${pkgbase}-headers")
for _p in ${pkgname[@]}; do
  eval "package_${_p}() {
    _package${_p#${pkgbase}}
  }"
done
