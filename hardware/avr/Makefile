TOPDIR ?= ../..

ifneq ($(TEENSY_SUPPORT),y)
$(ARCH_AVR)_SRC += hardware/avr/dump_ecmd.c
$(ARCH_AVR)_SRC += hardware/avr/fuse.c
$(ARCH_AVR)_SRC += hardware/avr/hostname.c

$(ECMD_EEPROM_SUPPORT)_SRC += hardware/avr/eeprom_ecmd.c

ifneq ($(DISABLE_REBOOT_SUPPORT),y)
$(ARCH_AVR)_SRC += hardware/avr/reset_ecmd.c
endif
endif

$(ARCH_AVR)_SRC += hardware/avr/bootloader_ecmd.c

##############################################################################
# generic fluff
include $(TOPDIR)/scripts/rules.mk

