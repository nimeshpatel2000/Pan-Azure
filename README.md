# Pan-Azure
This ARM template creates and bootstraps 2 VMSeries firewalls into an availability set.

Prerequisites:
1. Storage account created for the bootstrap files
2. Bootstrap folder setup, with init-cfg.txt and bootstrap.xml files in the "config" folder.

The template will deploy a VNET with network address 10.19.0.0/16 and the following subnets:

1. 10.19.0.0/24 - for management interface
2. 10.19.1.0/24 - for untrust interface
3. 10.19.2.0/24 - for trust interface
