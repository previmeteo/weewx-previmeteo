Weewx extension 
====

Send weather station data to Previmeteo.

Installation instructions
----

1) run the installer :

```
setup.py install --extension weewx-previmeteo.tgz
```

2) modify weewx.conf:

```
[StdRESTful]
    [[Previmeteo]]
        station = STATION_ID
        password = PASSWORD
```

3) restart weewx

```
sudo service weewx stop
sudo service weewx start
```
