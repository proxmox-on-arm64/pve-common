
PREFIX=/usr
BINDIR=${PREFIX}/bin
MANDIR=${PREFIX}/share/man
DOCDIR=${PREFIX}/share/doc
MAN1DIR=${MANDIR}/man1/
PERLDIR=${PREFIX}/share/perl5

LIB_SOURCES = \
	ACME.pm \
	ACME/Challenge.pm \
	ACME/StandAlone.pm \
	AtomicFile.pm \
	Certificate.pm \
	CLIFormatter.pm \
	CLIHandler.pm \
	CalendarEvent.pm \
	CpuSet.pm \
	Daemon.pm \
	Exception.pm \
	INotify.pm \
	JSONSchema.pm \
	Network.pm \
	OTP.pm \
	PTY.pm \
	ProcFSTools.pm \
	RESTEnvironment.pm \
	RESTHandler.pm \
	SafeSyslog.pm \
	SectionConfig.pm \
	Subscription.pm \
	Syscall.pm \
	Systemd.pm \
	Ticket.pm \
	Tools.pm

all:

.PHONY: install
install:
	install -d -m 0755 ${DESTDIR}${PERLDIR}/PVE
	install -d -m 0755 ${DESTDIR}${PERLDIR}/PVE/ACME
	for i in ${LIB_SOURCES}; do install -D -m 0644 PVE/$$i ${DESTDIR}${PERLDIR}/PVE/$$i; done


.PHONY: clean
clean: 	
	rm -rf *~ 

.PHONY: distclean
distclean: clean

