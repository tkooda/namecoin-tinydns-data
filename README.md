namecoin-tinydns-data
=====================

Generate tinydns DNS data file for namecoin's *.bit TLD



INSTALL WITH:
-------------

```
  git clone https://github.com/tkooda/namecoin-tinydns-data
  cd namecoin-tinydns-data/
  sudo python setup.py install
```


EXAMPLE USAGE:
--------------

```
  cd /service/tinydns/root/
  sudo namecoin-tinydns-data http://MyUsername:MyPassword@127.0.0.1:8336 1.2.3.4 > data
  sudo make
```

(presuming 'tinydns' is already supervised/running on "1.2.3.4") :
