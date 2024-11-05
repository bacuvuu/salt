# Useful salt scripts.

1. One-line bootstrap only master onedir saltstack with custom repo.
```bash
curl -L https://github.com/saltstack/salt-bootstrap/releases/latest/download/bootstrap-salt.sh | bash -s -- -M -N -R mirror.yandex.ru/mirrors/repo.saltproject.io onedir
```
2. One-line bootstrap minion onedir saltstack with custom repo.
```bash
 salt-ssh '*' -r 'wget -O - https://github.com/saltstack/salt-bootstrap/releases/latest/download/bootstrap-salt.sh | sudo sh -s -- -R mirror.yandex.ru/mirrors/repo.saltproject.io onedir'
```
