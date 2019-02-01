Vessel is a open source shell script for managing PHP development environment and related softwares such as databases, cache, application server and dns configurations on OSX.

## Getting Started

Once you have Vessel installed he will handle the installation of the latest version of:
- PHP
- Xdebug
- MySQL
- MongoDB
- NGINX
- Redis
- DNSMasq

## Installing Vessel

```
sudo curl -s https://raw.githubusercontent.com/jackmiras/vessel/master/install | bash
```

## Using Vessel

### Install the software previously described:

```
vessel --install
```

NOTE: All thoses software will be installed at once.

### Link project to NGINX:

1. Acces the project directory.

```
cd ~/Project/someproject
```

2. Link to NGINX.

```
vessel --link
```

Once the project has been linked you will he able to access him by using the project name with `.test` suffix.

Eg: `http://someproject.test`

### Unlink project from NGINX:

1. Acces the project directory.

```
cd ~/Project/someproject
```

2. Unlink from NGINX.

```
vessel --unlink
```

### To uninstall the softwares previously described:

```
vessel --cleanup
```

### To completely uninstall Vessel including the software, execute the following command:

```
sudo curl -s https://raw.githubusercontent.com/jackmiras/vessel/master/uninstall | bash
```

### Table of commands:

| Commands  | Description                                                                      |
|-----------|----------------------------------------------------------------------------------|
| --install | Installs PHP, Xdebug, MySQL, MongoDB, NGINX, Redis and DNSMasq.                  |
| --cleanup | Uninstall all the software described above and theirs respective configurations. |
| --link    | Link a Laravel project with NGINX.                                               |
| --unlink  | Unlink a Laravel project with NGINX.                                             |
| start     |  Start all the services related with the softwares intalled.                     |
| stop      |  Stop all the services related to the software installed.                        |
| restart   | Restart all the services related to the software installed.                      |
| status    | Show the status of the services related to the software installed.               |
