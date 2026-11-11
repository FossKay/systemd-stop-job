# systemd-stop-job
A note to self: how to change systemd stop job time

First, in `/etc/systemd/system.conf`, uncomment the line that about `DefaultTimeoutStopSec` and change it to `DefaultTimeoutStopSec=10s`.

Then, run `sudo systemctl daemon-reexec`.
