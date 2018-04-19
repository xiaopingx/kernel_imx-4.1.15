ifeq ($(CONFIG_OF),y)

dtb-$(CONFIG_SOC_IMX6Q) += \
	imx6dl-sabreauto.dtb \
	imx6dl-sabreauto-ecspi.dtb \
	imx6dl-sabreauto-enetirq.dtb \
	imx6dl-sabreauto-flexcan1.dtb \
	imx6dl-sabreauto-gpmi-weim.dtb \
	imx6dl-sabrelite.dtb \
	imx6dl-sabresd.dtb \
	imx6dl-sabresd-btwifi.dtb \
	imx6dl-sabresd-hdcp.dtb \
	imx6dl-sabresd-ldo.dtb \
	imx6dl-sabresd-enetirq.dtb \
	imx6q-sabreauto.dtb \
	imx6q-sabreauto-ecspi.dtb \
	imx6q-sabreauto-enetirq.dtb \
	imx6q-sabreauto-flexcan1.dtb \
	imx6q-sabreauto-gpmi-weim.dtb \
	imx6qp-sabreauto.dtb \
	imx6qp-sabreauto-ecspi.dtb \
	imx6qp-sabreauto-flexcan1.dtb \
	imx6qp-sabreauto-gpmi-weim.dtb \
	imx6qp-sabresd.dtb \
	imx6qp-sabresd-btwifi.dtb \
	imx6qp-sabresd-hdcp.dtb \
	imx6qp-sabresd-ldo.dtb \
	imx6q-sabrelite.dtb \
	imx6q-sabresd.dtb \
	imx6q-sabresd-btwifi.dtb \
	imx6q-sabresd-hdcp.dtb \
	imx6q-sabresd-ldo.dtb \
	imx6q-sabresd-enetirq.dtb \
	tideal.dtb
endif

DTB_NAMES := $(subst $\",,$(CONFIG_BUILD_ARM_APPENDED_DTB_IMAGE_NAMES))
ifneq ($(DTB_NAMES),)
DTB_LIST := $(addsuffix .dtb,$(DTB_NAMES))
else
DTB_LIST := $(dtb-y)
endif

targets += dtbs dtbs_install
targets += $(DTB_LIST)

always		:= $(DTB_LIST)
clean-files	:= *.dtb
