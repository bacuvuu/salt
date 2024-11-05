# Useful salt scripts.

1. One-line bootstrap onedir saltstack from custom repo.
```bash
 salt-ssh '*' -r 'wget -O - https://github.com/saltstack/salt-bootstrap/releases/latest/download/bootstrap-salt.sh | sudo sh -s -- -R mirror.yandex.ru/mirrors/repo.saltproject.io onedir'
```
