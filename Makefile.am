EXTRA_DIST = README.md

SUBDIRS = \
	minilzo \
	services \
	daemon \
	client \
	doc \
	suse \
	compilerwrapper

dist-hook:
	git log --date=short --pretty="format:@%cd  %an  <%ae>  [%H]%n%n%s%n%n%e%b" | sed -e "s|^\([^@]\)|\t\1|" -e "s|^@||" >$(distdir)/ChangeLog
