Planned downtime of dauntless
#############################

Due to the upgrade of our infrastructure, there will be a planned downtime for our virtualization host dauntless, with the following VMs and services affected:

- vm138 - crashtest
- vm152 - mail-test
- vm159 - mailhost-test
- vm165 - bibisect repos
- vm167 - bitgeria metrics
- vm171 - crashreport
- vm172 - online help mod
- vm173 - hc3 test
- vm174 - statistics
- win2k12r2

The downtime will be on Wednesday, April 20, 0730 UTC and last for about 30 Minutes.

Update
======

The downtime lasted about 150 Minutes due to the following problems that occured:

- During reboot, the RAID was not assembled as fast as expected by systemd. Fixed by adding rootdelay=10 to /etc/default/grub
- The network configuration with bridges was hard to adapt over kvm, and ifdown/ifup are not good enough for our complex network configuration, so a reboot was required.

