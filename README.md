# Magic mirror installer

This is an installer based on docker to configure your [Raspberry's Magic Mirror](https://github.com/nicolasgrancher/mirror).

## Install
### 0. Prerequisites
This installer use a docker-compose configuration. So you must have [docker](https://docs.docker.com/) running.

### 1. Clone repository
```git
git clone https://github.com/nicolasgrancher/mirror-installer.git
cd mirror-installer
```

### 2. Configure installer
```bash
cp .env.dist .env
vi .env
```
Edit `.env` config with your environment.

Note : There is a test container `rpi-test-image` for testing installation. You can use it with host `test`, port `22`

### 3. Run installer
```bash
docker-compose up
```

## Special thanks to...
William-Yeh for his Ansible container : https://hub.docker.com/r/williamyeh/ansible/

## TODO
- [ ] Make `rpi-test-image` work
- [ ] Test script with hardware
