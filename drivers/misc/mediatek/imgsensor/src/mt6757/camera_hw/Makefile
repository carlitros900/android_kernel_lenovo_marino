#
# Copyright (C) 2015 MediaTek Inc.
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License version 2 as
# published by the Free Software Foundation.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
# GNU General Public License for more details.
#

#
# Makefile for misc devices that really don't fit anywhere else.
#
ifneq ($(CONFIG_PINCTRL_MT6757),y)
# to use mtk legacy pinctrl
subdir-ccflags-y += -I$(DRVGEN_OUT)/inc
endif
MTK_CUSTOM_PATH  := $(srctree)/drivers/misc/mediatek
ifneq (, $(findstring marino, $(TARGET_PRODUCT)))
ccflags-y += -DCAMERAHW_INDRIYA
endif
ccflags-y += -I$(MTK_CUSTOM_PATH)/imgsensor/inc \

ifeq ($(CONFIG_L3510_MAINBOARD),y)
obj-y				+= kd_camera_hw.o
else
obj-y				+= kd_camera_hw_brady.o
endif
