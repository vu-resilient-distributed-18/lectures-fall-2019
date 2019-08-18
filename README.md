# Introduction

The goal of this class is to provide a foundation in the area of realiable distributed computing. This is specially important in order to be able to construct high assurance applications in this era of Internet of Things and Smart Cities. The technical landscape of the technologies in this area is changing rapidly: Memcached (a new kind of key-value store) has displaced standard file system storage, Chubby supports scalable locking and synchronization, ZooKeeper enables consistency-based  distributed services. Big Table manages sparse but enormous data sets. ZeroMQ. MQTT and DDS provide the reliable communication services. 

# Getting Started

In the initial part of this class we will use two linux virtual machines. Follow the instructions at https://github.com/RIAPS/riaps-integration/blob/master/riaps-x86runtime/README.md and load two virtual machines on your computer. When you are importing ensure that you reset the network interface addresses.

Ignore the instructions given in the subsection on "Securing Communication Between the VM and BBBs" because you will not be using beaglebones. 

## Alternative - Using Amazon EC2

**Guide to getting started with Amazon Web Services**

Adopted from: <https://aws.amazon.com/ec2/getting-started/>

**Step 1: Setting up AWS educate account**

-   Use this link <https://aws.amazon.com/education/awseducate/> and
    join aws educate. Please use your Vanderbilt email to create an aws
    educate account.

**Step 2: Getting into the AWS account**

-   Once you are approved of the account, please use this link
    <https://aws.amazon.com/education/awseducate/> to sign into to the
    AWS educate dashboard.

-   In the dashboard please select “**AWS Account**” and then “**Go to
    your AWS Educate starter kit**”

-   Then on the right top corner select “**Start Lab**”, this will take
    a couple of minutes the first time.

    (Do not “**End Lab**”, if you do so, you will lose all the data and
    instances you are using)

-   Once done choose “**Open Console**” on the left side, this will land
    you into the AWS services Dashboard.

**Step 3: Configure your instance**

-   Select “**EC2**” from the AWS services dashboard.

-   Then select the “**Launch instance**” option.

-   You have a few free instances which can be selected and used. For
    the assignments we will require the instance of “**Ubuntu 16.04
    LTS**”. Select the one with free tier eligible.

-   Select the security group, memory and other requirements for your
    instance.

-   Then click on “**Launch**” your instance. It will ask for a key
    pair.

-   Create a key pair: Select “**Create a new key pair**” and assign it
    a name you want. The key pair file (.pem) will be downloaded, save
    this file as you will require it every time you log in to the
    instance.

-   Finally, choose “**Launch Instances**” to complete the set up.

Note: It will take a few minutes to initialize your instance.

**Step 4: Connect to your instance**

-   Once your instance has been approved and ready to use, you can
    connect to your instance using PUTTY.

-   Install PUTTY using this link <https://www.putty.org/>

-   Now on your AWS dashboard you can see that your instance is running
    and after you see this select “**connect**”, this will prompt a page
    with instructions to connect to your instance using PUTTY.

-   Follow these instructions and use the public DNS provided to connect
    to your instance.

-   By default the password for the Ubuntu instance is **ubuntu**. Type
    in this password if prompted.

-   Following all these steps will get you into the Ubuntu instance.
    After you get in, you could install things similar to what you do on
    your laptop.

**Step 5: Terminate instances**

AWS EC2 instance can be used up to 750 hours/ month for free. If you
exceed this, **you will be charged** **as per their pricing in this
link** <https://aws.amazon.com/ec2/pricing/>

Select the EC2 instance, choose “**Actions**”, select “**Instance
State**”, and “**Terminate**” (if you are not using the instance
anymore). Terminate will delete your instance and data from AWS. So, for
short time use of instances you can “**STOP**” the instance.


# Reading Material

 * Textbook: Download from https://link.springer.com/book/10.1007/978-1-4471-2416-0 The book is available for free download from vanderbilt campus.
 * In addition to the textbook we will be assigning several reading materials for the class. 
 
# Class Discussion

 * Class discussion is going to be an important part of this course. I will be assigning papers for class discussion and the discussion will have to be lead by one of the students. 
 

# Syllabus

The course is going to be divided into 5 modules. Each module will end with an assignment and a report on the topic.  

* Module 1: Review of Networking - We will review the concept of sockets, internet
routing, TCP/UDP and DNS. These concepts are the backbone of distributed systems.
* Module 2:  Internet of Things and cloud - We will review internet of things, including the different distributed
application interaction patterns, for example pub/sub, synchronous and asynchronous
point to point communication. You will learn to use or review the use of MQTT,
REST/Websocket and ZeroMQ, DDS in this module. Towards the end of this module
you will build a vehicle-to-vehicle (V2V) communication network between cars in a
simulated environment called TORCS.
* Module 3: Understanding performance bottlenecks, Quality of Service and Failures - In this module we will review what is quality of service, how is it expressed and what
failure means.  It will be important to understand the concept of time synchronization. Additionally, during this module you will get introduced to the FMECA analysis and
will have to analyze the failure modes of the distributed application you have built
during the second module.
* Module 4: Reliability in Distributed systems – In this module you will be introduced
to formal concepts related to reliability in distributed computing systems. We will
discuss various techniques for overcoming failures, and achieving consistency,
availability, and reliability in distributed systems. We will be using the guide to reliable
distributed distributed systems book https://link.springer.com/book/10.1007/978-1-4471-2416-0 for the majority of this module and the next modules to follow.
* Module 5: Reliability techniques and related technologies – In this last module we
discuss several tools and techniques to retrofit reliability to complex systems. We will
review concepts of security schemes, clock synchronization, and transaction schemes
that are used to achieve reliability in practical distributed systems. At the end of this
module you will be able to apply these reliability concepts to the car’s V2V network
assignments.
* Tutorial and experience with [resilient information architecture platform for Smart Grid](https://riaps.isis.vanderbilt.edu) - This will be an invitation based 3 hour tutorial for you. You will be able to see how all the concepts we discussed in the class are implemented in practice. This will be an exciting tutorial and I encourage you to attend it.
* Final Project- the final module for this course is going to be a project, which you will develop
in teams.

