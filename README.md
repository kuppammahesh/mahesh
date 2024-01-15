 Q . WHAT IS AWS VPC ?
A . Amazon Virtual Private Cloud (Amazon VPC) is a service that lets you launch AWS resources in a logically isolated virtual network that you define. you can control your virtual network like your own IP address, subnets, configuration of route tables, and Gateways

Q . WHAT ARE THE CONNECTIVITY OPTIONS FOR MY VPC ?
A . INTERNET(via internet gateway)
     Your Corporate Data CenterUsing Hardware VPN(via virtual private gateway)
     Both Internet & Corporate datacenter(using internet gateway & virtual private gateway)
     Other AWS services(via internet Gateway,NAT,VPC Endpoints)
     Other VPC's

Q . HOW DO YOU CONNECT MY VPC TO INTERNET ?
A . Amazon VPC supports the creation of internet gateway which enables AAmazon EC2 Instances in the VPC to directly acess the internet

Q . WHAT ARE THE COMPONENTS OF AMZON VPC ?
A . VPC , SUBNET , INTERNET GATEWAY , NAT GATEWAY , HARDWAARE VPN CONNECTION , VIRTUAL      PRIVATE GATEWAY , ROUTER , CUSTOMER GATEWAY , PEERING CONNECTIONS . VPC ENDPOINT FOR S3

Q . STEPS TO BUILD CUSTOM VPC ?
A . CREATE VPC 
     CREATE SUBNETS
     CREATE AN INTERNET GATEWAY
     ATTACH INTERNET GATEWAY TO YOUR VPC
     CREATE NEW ROUTE TABLE
     ADD IG AS A ROUTE TO NEW RT
     ADD SUNEBTS TO RT SUBNET ASSOCIATION
     CREATE WEB SERVER(PUBLIC SUBNET) & DATABASE SERVER(PRIVATE SUBNET) INSTANCES
     CREATE NEW SECURITY GROUPS FOR NAT INSTANCE
     ADD HTTP & HTTPS INBOUND RULES THAT ALLOWS TRAFFIC FROM PRIVATE SUBNEST
     CREATE NAT INSTANCE(PUBLIC SUBNET)
     COMMUNITY AMI'S
     SEARCH FOR AMAZON-AMI-VPC-NAT CHOOSE FIRST IMAGE
     DISABLE AUTO ASSIGN PUBLIC IP
     ADD IT TO NAT SECURITY GROUP
     CREATE ELASTIC IP
     ASSOCIATE ELASTIC IP TO NAT
     DISABLE SOURCE/DESTINATION CHECKS FOR NAT
     ADD NAT INSTANCE AS A ROUTE TO INITIAL VPC RT

Q . ADVANTAGE OF USING AWS VPC ?
A . To build a virtual network in AWS cloud - no VPN , Hardware , physical Data center required , You      can define your own network space and control how your netwok and the amazon EC2 resources      inside youe network is exposed to the internet

Q . DIFFERENCE BLW STATEFUL AND STATELESS FILTERING ?
A . The most basic type of firewalls perform what is called stateful packet filtering, which means that      they can remember which side initiated the connection, and rules (called access control lists, or      ACLs) can be created based not only on IPs and ports but also depending on the state of the      connection 

    Stateless means that that state is managed by another system. On AWS, this can be DynamoDB, RDS,     S3, or other storage services. Managing a stateless system is less complex than managing a stateful         system. You can terminate single instances at any time without loosing data.

Q . CAN AMAZON EC2 INSTANCE WITH IN A VPC COMMUNICATES WITH AMAZON EC2 INSTANCE NOT       WITH IN VPC ? 
A . YES 

Q . CAN YOU USE YOUR EXISTING AMI'S IS AMAZON VPC ?
A . You can use AMI'S in Amazon VPC that are registered with in the same region





    
 
 
  
               
                          
    
       
       
                             
 
                 
 

   
    
