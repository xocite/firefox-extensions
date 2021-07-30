# Makefile for List Tabs

FILES = manifest.json \
        background.js \
        buildpage.js \
				page.html \
				style.css \
        $(wildcard icons/*.svg) \
        $(wildcard icons/*.png)

ADDON = listtabs

VERSION = $(shell sed -n  's/^  "version": "\([^"]\+\).*/\1/p' manifest.json)

trunk: $(ADDON)-trunk.xpi

release: $(ADDON)-$(VERSION).xpi

%.xpi: $(FILES)
	@zip -9 - $^ > $@

clean:
	rm -f $(ADDON)-*.xpi
