# DHCP-based User ID

This is for when there is no usable method to map users to IP addresses,
or when you want something simple for your home or non-production network.
MAC addresses and hostnames can be useful identifiers, which persist
across IP address changes. For this method to work, the PAN-OS device
needs to be the DHCP server, as it forwards the DHCP logs back to its
management interface, and parses out the MAC address/hostname to be used
as the "user" in the User-ID table. A customer wanted to use the idea of
presenting MAC addresses or hostnames as User-ID mappings in a
non-production environment