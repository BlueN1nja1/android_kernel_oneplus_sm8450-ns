# SPDX-License-Identifier: GPL-2.0
#
# Makefile for the Linux Kernel SOC specific device drivers.
#

obj-y				+= apple/
obj-y				+= aspeed/
obj-$(CONFIG_ARCH_AT91)		+= atmel/
obj-y				+= bcm/
obj-$(CONFIG_SOC_CANAAN)	+= canaan/
obj-$(CONFIG_ARCH_DOVE)		+= dove/
obj-$(CONFIG_MACH_DOVE)		+= dove/
obj-y				+= fsl/
obj-y				+= fujitsu/
obj-$(CONFIG_ARCH_GEMINI)	+= gemini/
obj-y				+= hisilicon/
obj-y				+= imx/
obj-y				+= ixp4xx/
obj-$(CONFIG_SOC_XWAY)		+= lantiq/
obj-$(CONFIG_LITEX_SOC_CONTROLLER) += litex/
obj-y				+= loongson/
obj-y				+= mediatek/
obj-y				+= microchip/
obj-y				+= nuvoton/
obj-y				+= pxa/
obj-y				+= amlogic/
obj-y				+= qcom/
obj-y				+= renesas/
obj-y				+= rockchip/
obj-$(CONFIG_SOC_SAMSUNG)	+= samsung/
obj-y				+= sifive/
obj-y				+= sunxi/
obj-$(CONFIG_ARCH_TEGRA)	+= tegra/
obj-y				+= ti/
obj-$(CONFIG_ARCH_U8500)	+= ux500/
obj-$(CONFIG_PLAT_VERSATILE)	+= versatile/
obj-y				+= xilinx/

obj-y     += oplus/storage/

#ifdef OPLUS_FEATURE_MM_FEEDBACK
obj-$(CONFIG_OPLUS_FEATURE_MM_FEEDBACK)	+= oplus/multimedia/
#endif /* OPLUS_FEATURE_MM_FEEDBACK */

#ifdef OPLUS_FEATURE_TP_BASIC
obj-$(CONFIG_OPLUS_DEVICE_IFNO)  +=  oplus/device_info/
#endif /* OPLUS_FEATURE_TP_BASIC */

$(warning MSM_ARCH: -$(MSM_ARCH)-)
ifneq ("$(MSM_ARCH)X", "waipio_tuivmX")
#ifdef OPLUS_FEATURE_SENSOR_SMEM
obj-y                       += oplus/sensor/
#endif /* OPLUS_FEATURE_SENSOR_SMEM */
endif

#ifdef CONFIG_OPLUS_SENSOR_CONSUMER_IR
obj-$(CONFIG_OPLUS_SENSOR_CONSUMER_IR_CORE) += oplus/oplus_consumer_ir/
#endif /* CONFIG_OPLUS_SENSOR_CONSUMER_IR */


#ifdef OPLUS_DFR_FEATURE
obj-y += oplus/dfr/
#endif /* OPLUS_DFR_FEATURE */

#ifdef OPLUS_FEATURE_MIDAS_GKI
obj-$(CONFIG_OPLUS_FEATURE_MIDAS_GKI) += oplus/power/midas/
#endif

#ifdef OPLUS_FEATURE_DFT
obj-y += oplus/dft/
#endif /* ifdef OPLUS_FEATURE_DFT */

#ifdef OPLUS_FEATURE_BOOT
obj-y += oplus/boot/
#endif /* OPLUS_FEATURE_BOOT */

$(warning MSM_ARCH: -$(MSM_ARCH)-)
ifneq ("$(MSM_ARCH)X", "waipio_tuivmX")
#ifdef OPLUS_FEATURE_MDMFEATURE
obj-$(CONFIG_OPLUS_FEATURE_MDMFEATURE)     += oplus/mdmfeature/
#endif /*OPLUS_FEATURE_MDMFEATURE*/
endif

#ifdef OPLUS_FEATURE_MODEM_MINIDUMP
obj-$(CONFIG_OPLUS_FEATURE_RECORD_MDMRST)     += oplus/mdmrst/
#endif /*OPLUS_FEATURE_MODEM_MINIDUMP*/

#ifdef OPLUS_SUBSYS_SLEEP_MONITOR
obj-$(CONFIG_OPLUS_SUBSYS_SLEEP_MONITOR)     += oplus/power/subsys_sleep_monitor/
#endif /* OPLUS_SUBSYS_SLEEP_MONITOR */

#ifdef OPLUS_FEATURE_THERMAL_HORAE
obj-$(CONFIG_HORAE_THERMAL_SHELL) += oplus/thermal/
#endif /* OPLUS_FEATURE_THERMAL_HORAE */
