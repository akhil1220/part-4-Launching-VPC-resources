# Part-4-Launching-VPC-resources
# Overview #
Launching EC2 instances in public and private subnets.
# Architecture #
<pre>
</pre>



# Steps #
 Used the resources which i have create in my previous projects. So far i had VPC with private and public subnets with routing tables cnnected to Internet gate way and Network ACLs for both public and private and a security group.
## EC2 INSTANCE FOR PUBLIC SERVER ##

1. I have created a *EC2 instance for my public subnet first*. To launch the instance i have created a name first and then selceted **Amazon linux for AMI**.
   
(AMI stands for Amazon Machine Image, and it's very similar to those pre-built computers. An AMI is a template or blueprint used to create EC2 instances and contains the operating system along with the applications needed to launch the instance. it gives prebuilt software and operating system.)

2. Then i selected a **instance type**. (Instance type covers hardware components.)
3. Now i created a key pair.
4. Next in networking panel i have changed settings and and ade sure this instance is connected to my own public subnet.
5. For public subnet i have already created a security group so here i used the existing security group.
6. Then clicked launch instance. The instance is launched.

## EC2 INSTANCE FOR PRIVATE SERVER ##
1. Created another EC2 instance and named the instance. Selected AMI instance type and here im using same key pair i created for public instance.
2. Now i have attached this instance to the private subnet,
3. Here im creating a security group because i did not create before as i did for public server.
4. So now im creating a security group then for inbound security group change type to SSH and source type to custom and in source add public security group  Choosing the Public Security Group as the source means only resources that are part of the Public Security Group can communicate with your instance.
5. Now i clicked launch instance. finally the instance is launched.


## SCREENSHOTS ##

## *PUBLIC EC2 INSTANCE* ##

<img width="2928" height="1210" alt="Image 11-17-25 at 2 51 AM" src="https://github.com/user-attachments/assets/3864c699-27e2-409a-95c6-70944e017e26" />




<img width="2684" height="828" alt="F32E7963-A6E6-483B-B535-4B3133433129" src="https://github.com/user-attachments/assets/690f078d-1cbb-4c7f-aa56-c6279fb0f8e7" />


## *PRIVATE EC2 INSTANCE* ##

<img width="2856" height="1148" alt="Image 11-17-25 at 6 42 AM" src="https://github.com/user-attachments/assets/aa067c71-a1cc-449a-b1eb-20754811cd83" />


<img width="2882" height="1276" alt="Image 11-17-25 at 6 43 AM" src="https://github.com/user-attachments/assets/611ab422-ec39-4d91-a086-1b0babb62c74" />


<img width="2790" height="862" alt="Image 11-17-25 at 6 43 AM (1)" src="https://github.com/user-attachments/assets/4708154d-fa4c-468b-ab12-c3e62098e2dd" />



