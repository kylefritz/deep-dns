# Deep DNS

Send deepmountain.com to 10.0.1.2

```
$ bundle
$ sudo ruby dns.rb
```

## Runbook

Network Name: Deep Mountain

get IP address of "server":
```
ifconfig | grep "inet " | grep -Fv 127.0.0.1 | awk '{print $2}'
```

create-react-app server can run on 80 and binds to 0.0.0.0 for public traffic
                        can proxy the rails app too (assumed running on 3000)
```
$ npm run live # starts on 80; requires sudo
```

## Tips

Bind any running servers to 0.0.0.0 (not localhost) so that *anyone* can connect
