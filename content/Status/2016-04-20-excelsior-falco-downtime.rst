Migration of Excelsior and Falco
################################

For the migration of our virtualization servers to our own rack and the upgrade to 10G based Intranet, we plan the downtime of excelsior on April 26, 0730UTC, and the downtime of falcon on April 27, 0730UTC. The downtime should last about one hour.
The vms that will be affected are:

Excelsior - April 26, 0730UTC
=============================

- vm134 - silverstripe staging
- vm136 - CentOS 64Bit Buildbot
- vm141 - Plone Test
- vm144 - Bugzilla Test instance
- vm146 - Askbot
- vm151 - tdf.io URL shortener
- vm156 - testwiki
- vm161 - blog
- vm162 - infra-testbed
- vm163 - wiki-test
- vm164 - officeshots
- vm166 - Windows 64Bit Tinderbox
- vm169 - pootle
- vm170 - graylog

Falco - April 27, 0730UTC
=========================

- vm137 - CentOS 32bit buildbot
- vm139 - Callgrind vm
- vm140 - Callgrind vm
- vm142 - dev-downloads
- vm143 - devcentral,perf
- vm145 - jenkins
- vm147 - moztrap
- vm148 - gerrit
- vm150 - bugzilla
- vm160 - floyd - saltmaster
- vm177 - CentOS 6 baseline 32bit
- vm178 - gerrit-test
- vm186 - new downloadarchive
- centOS64bit


Update April 26, 0820UTC
========================

excelsior has been migrated. There are some slight issues regarding the intranet connection, all public services are available again.

Update April 26, 0830UTC
========================

The newly fitted network card for excelsior seems to have one faulty port. Excelsior needs to be shutoff again to replace the interface

Update April 26, 0845UTC
========================

A HDD on excelsior also failed during migration, it will be replaced during the second downtime.

Update April 26, 1110 UTC
=========================

Excelsior is up and running.