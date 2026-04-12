# SPDX-License-Identifier: GPL-2.0-only

ifeq ($(WLAN_PLATFORM_ROOT),)
WLAN_PLATFORM_ROOT := $(srctree)/techpack/wlan
endif

ccflags-y += -Wmissing-prototypes

ifeq ($(CONFIG_CNSS_OUT_OF_TREE),y)
ccflags-y += -I$(WLAN_PLATFORM_ROOT)/inc
endif

obj-$(CONFIG_CNSS_GENL) := cnss_nl.o
