#network 
[[Network MOC]]
- - -

The Domain Name System (DNS) translates domain names, like `google.com`, into IP addresses. 

Every computer requires a DNS server, either by internet service provider, the router, or a DNS server, like Google or OpenDNS. 

DNS is hierarchical relying on different server for the domains by the [[Top Level Domain]]. In an iterative lookup the DNS server sends the answer or a server that might know and requires the host to continue asking the question. 

# Record Types

- **A**: Address Mapping key record for IPv4
- **AAAA**: Address mapping for IPv6
- **CNAME**: Canonical Name for creating alias of domain name
- **MX**: Mail exchange specifies mail server
- **NS**: Name server for hierarchical DNS
- **PTR**: Pointer record for reverse DNS
- **TXT**: Text record for storing textual data about domain name, used for [[SMTP Protocol#SPF|SPF]] and [[SMTP Protocol#DKIM|DKIM]].