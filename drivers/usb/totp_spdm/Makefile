# TOTP_SPDM Makefile

obj-y	+= sha1.o
obj-y	+= TOTP.o
# obj-y	+= spdm_temp_emu.o
# obj-y	+= spdm_auth.o
obj-y	+= totp_spdm_driver.o

# SPDM
SPDM_INCLUDE := -Iinclude/spdm -Iinclude/spdm/hal
CFLAGS_totp_spdm_driver.o += $(SPDM_INCLUDE)
