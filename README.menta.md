# pkg-mate-notification-daemon (Menta Linux)

Debian packaging of mate-notification-daemon 1.29.0 (Salsa packaging 1.26.1-1).
Upstream publishes no 1.29.0 release tarball, so the git tag archive
(`v1.29.0.tar.gz`) is used as the orig tarball; `autogen.sh` runs at build time.

Changes: `--enable-wayland` (gtk-layer-shell) and `--enable-in-process`
(do-not-disturb applet loaded in-process by mate-panel, required on Wayland);
installs the new autostart file; drops the applet's `.la`.

Versioning: `<upstream>-<debian rev>mentaN` (`1.29.0-1menta1`); bump with `dch -i`.
CI builds on push to `master`; tag `menta/<version>` also publishes a release.
