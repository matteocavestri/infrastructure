# Agetty TTY8 Autologin Admin --> Runit service

This service is used to start a user session on tty8 in order
to generate both `XDG_RUNTIME_DIR` and `DBUS_SESSION_BUS_ADDRESS` for the admin user.
This makes it possible for rootless Podman to function properly at startup.
