home-infra
==========

This is a repository that contains the basics to reconstitute my home
network in case of catestrophic failure (or hardware upgrade).

I've worked for SUSE for over 20 years so my home infrastructure revolves
around that ecosystem.  As a result, I've had the opportunity to improve
some of the ansible roles this setup uses.

dns_dhcp_home
-------------

This group defines the primary DNS/DHCP server node.  It sets up dhcp, dns for local zones plus TLS-encrypted forwarding to well-known servers, a wireguard endpoint, and telegraf telemetry targeting a local influxdb endpoint.
