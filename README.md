Use two themes for Grafana

endlessh-go - ID 15156
Node Exporter Dashboard EN 20201010-StarsL.cn - ID 11074

env and other things:

/grafana/.env
- ADMIN_USER=YOURUSER
- ADMIN_PASSWORD=YOURPASSWORD

/prometheus/prometheus/web.yml
basic_auth_users:
    admin: HASHEDPASSWORD

You can use generate_bcrypt_basic_auth.py to generate this password
