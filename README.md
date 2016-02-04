# Daily-Traffic-Limit-Warner
A simple daily traffic limit warner using vnstat and cron with bash

# Steps for application first running

- Install vnstat
```
sudo apt-get install vnstat
```

- Run `crontab -e` and copy the follow line into it
```
* * * * * env DISPLAY=:0 bash PATH_TO/limit-traffic >/dev/null 2>&1
```

- Set limit quote in `max` variable in MB