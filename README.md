# Network Subnetting Class (For Only Class C Networks)
Requirement: User has to provide full ip address (including CIDR) during instantiation in the form XXX.XXX.XXX.XXX/YY, where X represents IP Address, and Y represents CIDR

Attributes
---------------
IP: Extracts the IP Address from the Full IP Address provided by the User
CIDR: Extracts CIDR from the Full IP Address provided by the User
IP_Class: Gets IP Class for the provided Full IP
PartitionOctet: The Octet to be considered for partitioning 
bits: list of bits to be considered f


Methods
--------------


Constructor: parameter -> full_ip: IP Address with CIDR (Classless Inter-Domain Routing). e.g. 198.172.8.32/23 
  => assigns attributes and calls relevant local methods r t
