If you are using init, edit /etc/default/shadowsocks to switch between server mode and client mode.

If you are using systemd, you can manage your service by something like this:

systemctl status shadowsocks-server@server  # this will run in server mode, and using /etc/shadowsocks/server.json as config file
systemctl status shadowsocks-local@local  # this will run in client mode, and using /etc/shadowsocks/local.json as config file
