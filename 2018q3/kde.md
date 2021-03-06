## FreeBSD KDE status report ##

Contact: Adriaan de Groot <adridg@FreeBSD.org>, Tobias C. Berner <tcberner@FreeBSD.org>

Link:	 [KDE FreeBSD](https://freebsd.kde.org/)

KDE FreeBSD is responsible for the ports of the Plasma5 and KDE4 desktops, and
all associated applications. Further we also manage the Qt4 and Qt5 ports, as
well as cmake.

We also care for the FreeBSD builders for KDE's upstream CI on build.kde.org.

Since the last status report a lot of things have changed. First and foremost,
the Plasma5 Desktop and the Qt5 based KDE Applications have finally made their
way into the official ports tree after lingering for multiple years in our
development repository.

Secondly KDE4 has been marked deprecated and will be removed at the end of the
year. With Qt4 following no later than the next year (due to the exponentially
increasing burden of maintenance).

On a more technical side, bsd.qt.mk has been replaced by qt.mk and qt-dist.mk.
The porter's handbook is being updated (with thanks to Tobias Kortkamp).

Further we have been keeping cmake and Qt5 and almost every other port under our
control up to date. SDDM has been updated to the next-to-latest release with
backported security fixes.

One big issue we have is www/qt5-webengine, which requires too much time to keep
up to date, as the underlying chromium is in need of many patches, which change 
with every release. Another upcoming issue is the way in which FreeBSD's libinput
lags behind. This blocks future updates to KDE Plasma as well as Wayland 
improvements. Thankfully x11@ is looking at this issue already, so it should be
fixed soon -- for the meantime people who want to give the latest KDE Plasma
Desktop a try can use the appropriate branch from our github.

People who are willing to contribute can find us on #kde-freebsd on freenode,
the kde@FreeBSD.org mailing list. Further we accept pull-requests and
contributions on github.com/freebsd/freebsd-ports-kde.
