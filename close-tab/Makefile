# -*- Mode: Makefile -*-
#
# Makefile for Undo Close Tab
#

FILES = manifest.json \
        background.js \
        $(wildcard _locales/*/messages.json) \
        $(wildcard icons/*.svg) \
        $(wildcard icons/*.png)

ADDON = closetab

VERSION = $(shell sed -n  's/^  "version": "\([^"]\+\).*/\1/p' manifest.json)

trunk: $(ADDON)-trunk.xpi

release: $(ADDON)-$(VERSION).xpi

%.xpi: $(FILES)
	@zip -9 - $^ > $@

clean:
	rm -f $(ADDON)-*.xpi
