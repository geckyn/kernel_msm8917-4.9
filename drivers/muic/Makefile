#
# Makefile for muic devices
#

ifeq ($(CONFIG_MUIC_S2MU004),y)
	obj-y				+= muic_core.o s2mu004-muic.o s2mu004-muic-sysfs.o
	obj-$(CONFIG_CCIC_NOTIFIER)		+= muic_manager.o
else
	obj-y				+= muic-core.o
#	obj-$(CONFIG_MUIC_SUPPORT_CCIC)	+= universal/muic_ccic.o
endif

obj-$(CONFIG_MUIC_NOTIFIER)		+= muic_notifier.o
obj-$(CONFIG_MUIC_S2MU005)		+= s2mu005-muic.o
obj-$(CONFIG_MUIC_MAX77804)		+= max77804-muic.o
obj-$(CONFIG_MUIC_MAX77804K)		+= max77804k-muic.o
obj-$(CONFIG_MUIC_MAX77828)		+= max77828-muic.o
obj-$(CONFIG_MUIC_MAX77843)		+= max77843-muic.o
obj-$(CONFIG_HV_MUIC_MAX77843_AFC)	+= max77843-muic-afc.o
obj-$(CONFIG_MUIC_MAX77833)             += max77833-muic.o
obj-$(CONFIG_HV_MUIC_MAX77833_AFC)      += max77833-muic-afc.o
obj-$(CONFIG_MUIC_MAX77888)		+= max77888-muic.o
obj-$(CONFIG_MUIC_FSA9480)		+= fsa9480.o
obj-$(CONFIG_MUIC_S2MM001)		+= s2mm001.o
#obj-$(CONFIG_MUIC_UNIVERSAL)		+= universal/

ifeq ($(CONFIG_MUIC_HV),y)
obj-$(CONFIG_MUIC_S2MU004)	+= s2mu004-muic-afc.o
endif
