# Quick start SaltStack

#### One-line bootstrap `only master` onedir saltstack with custom repo.
```bash
curl -L https://github.com/saltstack/salt-bootstrap/releases/latest/download/bootstrap-salt.sh | bash -s -- -M -N -R mirror.yandex.com/mirrors/repo.saltproject.io onedir
```
#### One-line bootstrap minion onedir saltstack with custom repo from `salt-ssh`.

##### roster file example
```
salt-lab:
  host: 192.168.111.111
  user: salt-test
  passwd: test
  tty: True
```
##### command
```bash
salt-ssh '*' -r 'wget -O - https://github.com/saltstack/salt-bootstrap/releases/latest/download/bootstrap-salt.sh | sudo sh -s -- -R mirror.yandex.com/mirrors/repo.saltproject.io onedir'
```
#### Simple minion test

```bash
salt \* test.ping
```
#### line from `add-feature` branch
