# Proxy List

> A list of public HTTP proxy. Updated and tested daily. **See the file** `ProxyList.txt`.

## About

This list is an aggregation of several other resources of public proxy lists. Even proxies from online lists like `www.freeproxy.net` which were tested couple second ago didn't worked for me. The resource aggregation, the availability test and the list publishing is done every day.

### Why this list?

I wasn't able to find any easy-to-download and reliable resource of public proxies. So, I made one for myself.

### How is the availability of proxy tested?

A proxy must respond to request within 10 second and it has 3 attempts to do so. The target is `www.seznam.cz`. The second level is a random web server from a pool of server hosted by same provider. The third level is one particular Czech eshop.

### Is it guaranteed that the proxies from the list will work?

Nope. Any proxy from the `ProxyList.txt` can actually stop to work or stop to respond to requests anytime between the update interval.

### Where is the source code of the this proxy generator?

This proxy generator is created by PowerShell and its syntax is close-source hosted in one of my private repository.

## Release notes

### 2021-09-29

* Update backend to .NET 6 => **HTTPS, SOCKS** support ❗❗❗

### 2021-09-05

* Add 3rd level of verification (a response within 10 seconds to one czech eshop)
* Update 2nd level of verification (a response withing from 15 to 10 second)

### 2021-04-12

* Add ProxyBroker to the proxy generator to find some additional proxies from various resources

### 2021-04-11

* Add Pzzqz.com as a source of proxy
