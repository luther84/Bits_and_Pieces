root@emby:/etc/systemd/system/emby-server.service.d# pwd
/etc/systemd/system/emby-server.service.d
root@emby:/etc/systemd/system/emby-server.service.d# cat restart.conf
[Service]
Type=forking
GuessMainPID=true
Restart=on-failure
RestartSec=5s

