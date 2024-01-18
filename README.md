# Network Subnetting Class (For Only Class C Networks)
Requirement: User has to provide full ip address (including CIDR) during instantiation in the form XXX.XXX.XXX.XXX/YY, where X represents IP Address, and Y represents CIDR

Attributes
---------------
IP: Extracts the IP Address from the Full IP Address provided by the User  
CIDR: Extracts CIDR from the Full IP Address provided by the User  
IP_Class: Gets IP Class for the provided Full IP  
PartitionOctet: The Octet to be considered for partitioning   
bits: list of bits  [8, 16, 24, 32]  


Methods
--------------

1. Constructor: parameter -> full_ip: IP Address with CIDR (Classless Inter-Domain Routing). e.g. 198.172.8.32/23  
  => assigns attributes and calls relevant local methods  
2. check_fullIP_validity(): checks for the validity of IP address provided as argument  
3. findIPClass: checks and displays the Class of IP based on the Full IP provided    
4. retrieveOctetPosition(): gets the octet position to considered for the IP partitioning. would be useful in the subnetting class.  
  => parameter: >> cidr  
  => returns: >> the octet position (int)  
5. paddedZeroes(): pads the IP with zeroes starting from the partition point  
  => parameter: binaryNumberString (string)  
  => returns: padded ips (binaryNumberString)  
6. binaryToDecimal(): converts binary number (int) to base 10 (decimal) number  
  => parameter: binaryNumber (int)  
  => returns: decimalNumber (int)  
7. convertDecimalToAnotherBase(): converts base 10 (decimal) number to a given base numbber  
  => parameters: baseNumber (int) >> the base to convert to decimal number to
                numberToConvert (int) >> the number to be converted  
  => returns: baseString (string) >> the converted base number  
8. longIP(): converts IP to a long string (without the '.' seperator)  
  => parameter: IP (string) >> the IP to be converted    
  => returns: IPMerged (string) >> the long IP  
9. InsertDotInIP(): join separated octet ips  
    => parameter: longIP (string) (binary IP) >> the long IP  
   => returns: longIP with dots  
10. breakIPsIntoOctet(): breaks the IPs into octets and stores them in a list  
    => parameter: longIP  
    => returns: list of octet IPs  
11. findNetworkBroadcastandSubnetAddresses(): finds the network address and subnet address of a given network  
    => parameters: IP >> the IP address; cidr >> the CIDR of the network  
    => returns: networkAddress, broadcastAddress, subnetMaskAddress of the newtwork  
12. IPToBinary(): converts an IP to binary IP  
    => parameter: IP  
    => returns: binaryIP (string), octetList (List)  
13. findHostRange(): find the hosts in a network  
    => parameters: networkAddress; broadcastAddress  
    => returns: hosts  
14. replaceLastOctet(): replaces the last octet of an IP with last octets of the host IPs
    parameters: IP; newOctet
    returns: 
   
  
