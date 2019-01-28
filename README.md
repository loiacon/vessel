Vessel is a open source shell script for managing PHP development environment and related softwares such as databases, cache, application server and dns configurations on OSX.

## Getting Started

Once you have Vessel installed he will handle the installation of:
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

### Link project with NGINX:

1. Acces the project directory.

```
cd ~/Project/someproject
```

2. Link to NGINX.

```
vessel --link
```

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
