Weewx extension 
====

Send weather station data to Previmeteo.

Installation instructions
----

1) Get latest release

```
wget https://github.com/previmeteo/weewx-previmeteo/archive/v0.1.tar.gz -O weewx-previmeteo-v0.1.tar.gz
```

1) Run weewx extension installer

```
setup.py install --extension weewx-previmeteo-v0.1.tar.gz
```

2) Modify weewx.conf:

```
[StdRESTful]
    [[Previmeteo]]
        station = STATION_ID
        password = PASSWORD
```

3) Restart weewx service

```
sudo service weewx restart
```
