
# Research Topic Task 2


## Whats a VPC?

- Virtual Private Cloud (VPC) is an on-demand configurable pool of shared computing
resources allocated within a public cloud environment, providing a certain level
of isolation between the different organisations using the resources.

### Amazon VPC

- Amazon VPC lets you provision a logically isolated section of the AWS Cloud where
you can launch AWS resources in a virtual network that you define. You'll have complete
control over your virtual networking environment, including selection of your own IP
address range, creation of subnets, and configuration of route tables and network gateways.

Benefits Using Amazon VPC:
  - Secure: security groups and network access control lists, to enable inbound
  and outbound filtering at the instance and subnet level.
  - Simple: Able to create a VPC quickly and easily using the AWS Management Console.
  - Customise: Control your virtual networking environment, including selection of
  your own IP address range, creation of subnets, and configuration of route tables
  and network gateways.


## What are Subnets?

- A subnetwork or subnet is a logical subdivision of an IP network. The practice of
dividing a network into two or more networks is called subnetting.

An Example of a Subnets:

STEP 1:
```
IP Address  : 192.168.5.85
Subnet Mask : 255.255.255.0
```

STEP 2: Converting Decimals ---> Binary
```
IP Address  : 11000000. 10101000. 00000101. 01010101
Subnet Mask : 11111111. 11111111. 11111111. 00000000
```

STEP 3: A Comparison Between IP and Subnet Mask
```
IP Add : 11000000. 10101000. 00000101. 01010101
SubM   : 11111111. 11111111. 11111111. 00000000

AND    : 11000000. 10101000. 00000101. 00000000
```

## What are Private Subnets?

- Private Subnets consist of a private IP address, and they are usually behind a
firewall or router that performs NAT (Network Address Translation). They only supposed
to work within the local network.

## What are Public Subnets?

- Public Subnet has an Internet Gateway attached which is used by the EC2 instances
to access the internet.

## NACLs vs Security Groups? (Inbound and Outbound)

- Security Groups: adds a security layer to EC2 instances that control both inbound
and outbound traffic at the instance level.

- Network Access Control List or NACLs: adds an additional layer of security associated
with subnets that control both inbound and outbound traffic at the subnet level.

### Stateful vs Stateless.

- The key difference between stateful and stateless applications is that stateless applications
don't “store” data whereas stateful applications requires data to be stored.


## NAC rules for a our Node-Sample-App Public Subnet (Where do clients come in?)
## port 80... You want loggin to install stuff? Port 22... You need to communicate
## to db?

## NAC rules for a our Node-Sample-App DB - Private Siubnet (Where does traffic
##  come from?) and where does it need to go?
