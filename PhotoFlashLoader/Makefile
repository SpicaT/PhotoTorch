ifeq ($(SIMULATOR),1)
	TARGET = simulator:clang:latest
	ARCHS = x86_64 i386
else
	TARGET = iphone:latest:6.0
	ARCHS = armv7 arm64 arm64e
endif

include $(THEOS)/makefiles/common.mk

TWEAK_NAME = PhotoFlash
PhotoFlash_FILES = Tweak.xm

include $(THEOS_MAKE_PATH)/tweak.mk
