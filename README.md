SSL Config
==========

<a href="https://travis-ci.org/typesafehub/ssl-config"><img src="https://travis-ci.org/typesafehub/ssl-config.svg"/></a>

Goal and purpose of this library is to make Play's WS librari as well as Akka HTTP "secure by default".
Sadly, while Java's security has been steadily improving some settings are still left up to the user,
and certain algorithms which should never be used in a serious prodution system are still accepted by 
the default settings of the SSL/TLS infrastructure. These things are possible to fix, by providing specialized 
implementations and/or defining additional settings for the Java runtime to use – this is exactly the purpose of SSL Config.

Additional modules offer integration with Play WS (which by default utilises the Ning Async Http Client), 
Akka Http and any other library which may need support from this library.

Documentation
=============

Docs are available on: http://typesafehub.github.io/ssl-config

Recommended reading
===================

An excellent series by [Will Sargent](https://github.com/wsargent) about making
[Play's WS](https://www.playframework.com/documentation/2.4.x/ScalaWS) (from which this library originates) "secure by default":

- [Fixing the Most Dangerous Code in the World](https://tersesystems.com/2014/01/13/fixing-the-most-dangerous-code-in-the-world/)
- [Fixing X.509 Certificates](https://tersesystems.com/2014/03/20/fixing-x509-certificates/)
- [Fixing Certificate Revocation](https://tersesystems.com/2014/03/22/fixing-certificate-revocation/)
- [Fixing Hostname Verification](https://tersesystems.com/2014/03/23/fixing-hostname-verification/) 
- [Testing Hostname Verification](https://tersesystems.com/2014/03/31/testing-hostname-verification)

License
=======

Typesafe 2015, Apache 2.0
