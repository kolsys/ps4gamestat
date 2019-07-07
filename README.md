# ps4gamestat
PlayStation 4 usage statistics aggregator

# Installation

```
git clone 
git submodule init
git submodule update
```

Change DB_PATH and WEB_PORT variable if you needed.

# Runing

sudo -u www /INSTALLATION/PATH/ps4games PS4_IP\[ PS4_IP_2 ... PS4_IP_N\]
Open statistics in the browser: http://localhost:8054/

# Autostart
You can use systemd sysV for autostarting daemon on Linux.

For OSX change you PS4 host in `osx-run.plist` and add to autostart:
```
sudo install osx-run.plist /Library/LaunchDaemons/com.github.kolsys.ps4gamestat.plist
sudo launchctl load -w /Library/LaunchDaemons/com.github.kolsys.ps4gamestat.plist
```

