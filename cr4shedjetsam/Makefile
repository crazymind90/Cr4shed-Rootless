INSTALL_TARGET_PROCESSES = ReportMemoryException

include $(THEOS)/makefiles/common.mk

export THEOS_PACKAGE_SCHEME = rootless

TWEAK_NAME = Cr4shedJetsam
Cr4shedJetsam_FILES = $(wildcard *.xm *.mm ../Shared/*.mm) ../cr4shedmach/mach_utils.mm
Cr4shedJetsam_CFLAGS = -fobjc-arc -I../Include -Wno-unused-variable
Cr4shedJetsam_LDFLAGS += -F../Frameworks/ -L../Libraries/
Cr4shedJetsam_FRAMEWORKS = CoreSymbolication
Cr4shedJetsam_LIBRARIES = MobileGestalt
ADDITIONAL_CFLAGS += -DTHEOS_LEAN_AND_MEAN -Wno-shorten-64-to-32

include $(THEOS_MAKE_PATH)/tweak.mk
