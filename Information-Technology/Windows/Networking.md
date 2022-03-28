# Command Prompt

## Find all relevant client networking info
- ipconfig /all

## Remove client from the DHCP server list (caution: will lose external network access)
- ipconfig /release
### Add client back to DHCP server list
- ipconfig /renew

## Clear DNS & NetBIOS name resolutions on client computer
- ipconfig /flushdns
- nbtstat –R (requires administrator privileges)

## Trace the route to destination (note: useful when a destination takes multiple server hops to reach)
- tracert <dns_name or ip_address>

## Check connectivity
- ping <dns_name or ip_address>
### Show client and destination information (note: similar to tracert command)
- pathping <dns_name or ip_address>
### Consistent ping
- ping -t <dns_name or ip_address>
