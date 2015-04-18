capbash-git
==============

Scripts for extracting tarballs and zip compressed files.

# How to Install #

Install capbash first, more details at:
https://github.com/capbash/capbash

```
curl -s https://raw.githubusercontent.com/capbash/capbash/master/capbash-installer | bash
capbash new YOUR_REPO_ROOT
cd YOUR_REPO_ROOT
```

Now you can install git into your project

```
capbash install tarball
```

# Configurations #

The available configurations include:

```
TARBALL_BASE_DIR=${TARBALL_BASE_DIR-/var/local/apps}
TARBALL_NAME=${TARBALL_NAME}
TARBALL_FILENAME=${TARBALL_FILENAME}
```


# Deploy to Remote Server #

To push the git script to your server, all you need if the IP or hostname of your server (e.g. 192.167.0.48) and your root password.

```
capbash deploy <IP> tarball
```

For example,

```
capbash deploy 127.0.0.1 git
```
