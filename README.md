Cute little systemd automatic service restart unit

    root@emby:/etc/systemd/system/emby-server.service.d# pwd
    /etc/systemd/system/emby-server.service.d
    root@emby:/etc/systemd/system/emby-server.service.d# cat restart.conf
    [Service]
    Type=forking
    GuessMainPID=true
    Restart=on-failure
    RestartSec=5s
    
    
Added to ovpn file on Ubuntu 18.04 to allow proper search domain to be set
    
    script-security 2
    up /etc/openvpn/update-systemd-resolved
    down /etc/openvpn/update-systemd-resolved
    down-pre
