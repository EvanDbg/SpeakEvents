GO_EASY_ON_ME = 1

include theos/makefiles/common.mk

export TARGET=iphone:latest:5.0
export ARCHS = armv7 arm64

TWEAK_NAME = SpeakEventsSupport
SpeakEventsSupport_FILES = Tweak.xm
SpeakEventsSupport_FRAMEWORKS = MapKit
SpeakEventsSupport_PRIVATE_FRAMEWORKS = AppSupport VoiceServices

include $(THEOS_MAKE_PATH)/tweak.mk

distclean:
	rm *.deb || true

test: distclean package install
