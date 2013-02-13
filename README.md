namecoin-tinydns-data
=====================

Generate tinydns DNS data file for namecoin's *.bit TLD


REQUIRES:
---------
 - 'tinydns' installed and supervised as /service/tinydns/
   (http://cr.yp.to/djbdns/tinydns.html)


INSTALL WITH:
-------------

```
  git clone https://github.com/tkooda/namecoin-tinydns-data
  cd namecoin-tinydns-data/
  sudo python setup.py install
  sudo cp tinydns-Makefile /service/tinydns/root/Makefile
```


EXAMPLE USAGE:
--------------

```
  cd /service/tinydns/root/
  sudo make
```


ADDITIONAL HELP:
----------------
To be able to perform local DNS queries through a djbdns dnscache:
```
  ln -s /service/tinydns/env/IP /service/dnscache/root/servers/bit
  sv t /service/dnscache/
  echo 'nameserver 127.0.0.1' > /etc/resolv.conf
```
