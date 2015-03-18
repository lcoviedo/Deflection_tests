# Traffic deflection tests on XenServer

3 tests run into XenServer to compare host and guests performance with/without traffic deflection

## 1st Test - One VM

1 guest machine (A) receiving total traffic at rates of 2500, 5000, 10000, 15000, and 20000pps from 2 packet generators.

## 2nd Test - Two VMs

2 guest machines (A and B) running on the same XenServer host. 
A receiving traffic from a packet generator at rates of 1250, 2500, 5000, 7500, 10000, and 20000pps.
B receiving traffic from a different packet generator at rates of 1250, 2500, 5000, 7500, 10000, and 20000pp.
XenServer host is also measured.

## 3rd Test - Two VMs with Traffic Deflection

2 guest machines (A and B) running on the same XenServer host.
Traffic generators send traffic to guest A, OvSwitch redirects half of the traffic to guest B at rates of 1250, 5000, 10000, and 20000pps.
XenServer host is also measured.
