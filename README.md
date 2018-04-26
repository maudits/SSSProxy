SSSocks Proxy v0.1
=============================

SSSProxy is a socks interceptor proxy. It was originally created to work along with tsocks (or socat,depending on the circumnsances) and to allow interception and loggin of TCP data in a nice hexadecimal and ASCII view. 

This scirpt implements the very basic of a proxy server and it can be customised to extend its functionalities. It currently only support TCP traffic (SocksV4).

The following is an example of the the SSSProxy traffic view:
```
Mon Apr 22 20:45:48 2013        127.0.0.1:36699 > 4.2.2.2:53
00 25 E3 B2 01 00 00 01 00 00 00 00 00 00 08 6D .%.............m
63 75 70 64 61 74 65 06 74 75 6D 62 6C 72 03 63 cupdate.tumblr.c
6F 6D 00 00 01 00 01                            om.....

Mon Apr 22 20:45:53 2013        127.0.0.1:36701 > 4.2.2.2:53
00 25 2F D3 01 00 00 01 00 00 00 00 00 00 08 6D .%/............m
63 75 70 64 61 74 65 06 74 75 6D 62 6C 72 03 63 cupdate.tumblr.c
6F 6D 00 00 01 00 01                            om.....

Mon Apr 22 20:45:56 2013        127.0.0.1:36701 < 4.2.2.2:53
00 45 2F D3 81 80 00 01 00 02 00 00 00 00 08 6D .E/............m
63 75 70 64 61 74 65 06 74 75 6D 62 6C 72 03 63 cupdate.tumblr.c
6F 6D 00 00 01 00 01 C0 0C 00 01 00 01 00 00 00 om..............
19 00 04 42 06 24 30 C0 0C 00 01 00 01 00 00 00 ...B.$0.........
19 00 04 42 06 28 18                            ...B.(.

Mon Apr 22 20:46:10 2013        127.0.0.1:36703 > 4.2.2.2:53
00 25 9E DA 01 00 00 01 00 00 00 00 00 00 08 6D .%.............m
63 75 70 64 61 74 65 06 74 75 6D 62 6C 72 03 63 cupdate.tumblr.c
6F 6D 00 00 01 00 01                            om.....
```


