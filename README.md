openmagic
=========

OpenSSL TLS heartbeat read overrun (CVE-2014-0160)

Usage:

$ ./ssltest.sh login.foo.com 443
# [Open  ] login.foo.com:443 (1.2.3.5)
# [Vuln  ] login.foo.com:443
# [Loop  ] login.foo.com:443 %1
...
# [Loop  ] login.foo.com:443 %1000

$ ./sslmail.sh foobar.com
# [Closed] mx6.foobar.com:465
# [Closed] mx6.foobar.com:585
# [Open  ] mx6.foobar.com:993 (1.2.3.4)
# [Safe  ] mx6.foobar.com:993
# [Open  ] mx6.foobar.com:995 (1.2.3.4)
# [Safe  ] mx6.foobar.com:995
