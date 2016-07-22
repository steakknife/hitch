
SUBDIRS = src

hitch.8: hitch.man.rst
if FOUND_RST2MAN
	${RST2MAN} --halt=2 $(srcdir)/hitch.man.rst $@
else
	@echo "$@ is out-of-date but rst2man{,.py} was unavailable"
	@false
endif

doc_DATA = hitch.conf.example CHANGES.rst README.md

dist_man_MANS = hitch.8

EXTRA_DIST = LICENSE README.md hitch.man.rst hitch.conf.example CHANGES.rst docs
