### About
This is a docker setup for monitoring an SSH honeypot
![](https://github.com/shizunge/endlessh-go/raw/main/dashboard/screenshot.png)
This image and exporter written in golang was taken from [here](https://github.com/shizunge/endlessh-go)

### Grafana themes used

`15156` - endlessh-go

`11074` - Node Exporter Dashboard EN 20201010-StarsL.cn

### env and other things:

*/grafana/.env*
```
ADMIN_USER=YOURUSER
ADMIN_PASSWORD=YOURPASSWORD
```

*/prometheus/web.yml*
```
basic_auth_users:
    admin: HASHEDPASSWORD
```
You can use [generate_bcrypt_basic_auth.py](prometheus/generate_bcrypt_basic_auth.py) to generate this password
