Distributes IP addresses and leases to clients.

Tested successfully on Parrot OS. Smartphone client: Samsung Galaxy III. 

Configuration:
Specify network device (/etc/default/isc-dhcp-server)
Specify network range (/etc/dhcp/dhcpd.conf). Basic form: subnet netmask{}
Check ISC DHCP Server-configuration: config_check
Get PID for DHCP-service:get_pid
Check configuration, lease and PID-file in one operation:multi_check

Operation:
Start DHCP-service:server_start. Note: run ONLY if service not running.
Check DHCP-connections:connections_check
Check current leases:lease_check
Stop DHCP-service:server_stop

Files:
config_check
get_pid
multi_check
server_start
server_stop
lease_check

