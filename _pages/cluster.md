---
layout: archive
title: "Cluster"
permalink: /projects/cluster/
author_profile: true
redirect_from:
  - /projects/cluster
---

{% include base_path %}

The Little Cluster that Could
======

<img src="https://github.com/hbwddl/hbwddl.github.io/blob/master/images/cluster.jpg" height="400" width="300">

My little cluster, hanging out in my cabinet.

The Idea
------

My personal cluster began in 2017 when I discovered that the U sold entire computers (sans hard drives) for 30 dollars at their surplus store. Once I'd procured an entire extra computer, I needed something to do with it. I'd used one of UCLA's clusters during my BIG summer research experience, and I wanted to learn more about it.

I bought a refurbished hard drive, installed [Ubuntu](https://ubuntu.com/) on it, and started searching for easy ways to make a cluster. I tried ready-made HPC distros/packages such as [PelicanHPC](https://www.pelicanhpc.org/) and [KestrelHPC](http://kestrelhpc.sourceforge.net/). I wanted a clustering solution that could accommodate heterogeneous hardware (I had old computers), was open source, would allow me to install and primarily use parallel programming in R, and wasn't super difficult to install and maintain.

After three or so years of wrangling this cluster, I've finally settled on a setup that feels fun and usable for me. I've got four nodes in my cluster, and I'm currently running an [Apache Spark](https://spark.apache.org/) cluster, learning how to use Sparklyr for machine learning workflows. I've also got MPI capabilities on my cluster.

Much credit and appreciation to the following pages and guides:

[https://www.admin-magazine.com/HPC/Articles/Building-an-HPC-Cluster](https://www.admin-magazine.com/HPC/Articles/Building-an-HPC-Cluster)

[https://mpitutorial.com/tutorials/running-an-mpi-cluster-within-a-lan/](https://mpitutorial.com/tutorials/running-an-mpi-cluster-within-a-lan/)

[https://www.tutorialkart.com/apache-spark/how-to-setup-an-apache-spark-cluster/](https://www.tutorialkart.com/apache-spark/how-to-setup-an-apache-spark-cluster/)

Overall
------

Clustering seems a lot more complicated than it actually ends up being. The main advantages you get in setting up a personal cluster are twofold--you don't have to figure out a way to share cluster usage among multiple users, and you have full admin access to everything.

In this setup, then, setting up the infrastructure for your cluster is actually quite simple. Once you have physically networked all of your computers together, your cluster needs two things as a base:

* A way for your master node to give commands to the other nodes (I use passwordless ssh for this)

* A shared filesystem (I used NFS for this)

That's it! Things will get more complicated when you care about cluster sharing and job scheduling, but this is all you need to set up MPI or Spark.

Materials + Costs
------

#### Nodes

* Lenovo Ideapad U430p 
    * I had this laptop on hand already. I use it as the master node for my cluster.
    * 4gb RAM, 4 cores, 250GB hard drive
    * Ubuntu 20.04
    
* HP Compaq 8200 Elite SFF
    * $30, University of Utah
    * $18 refurbished 350gb WD hard drive, Newegg
    * 4gb RAM, 4 cores
    * Ubuntu 20.04
    
* HP Compaq 8300 Ultra SFF
    * $32, Ebay
    * Did not look carefully at the specs...needed an external power supply. $17 on Ebay.
    * $25, 128 GB Samsung EVO ssd, Newegg
    * 2gb RAM, 4 cores
    * Ubuntu 20.04
    
* HP Compaq 8000 Elite SFF
    * $42, Ebay ($16 shipping)
    * $25, 128 GB Samsung EVO ssd, Newegg
    * 8gb RAM, 4 cores
    * Debian Jessie (working on it! Kept getting a kernel panic when I attempted to install Ubuntu)
 

#### Networking

* Ethernet Switch, TP link
    * 5 ports
    * $15, Amazon
    
* Ethernet cables, 5 pack
    * $12, Amazon
    
* Wireless router, Linksys
    * I use this as an [ethernet bridge](https://smallbusiness.chron.com/convert-linksys-router-ethernet-bridge-57403.html#:~:text=Click%20the%20%22Connectivity%22%20link%20in,OK%22%20to%20enable%20bridge%20mode.) to connect my cluster to wifi.
    * Had this on hand

#### Other

* Monitor + VGA cable
    * $14, Goodwill
    
* Keyboard and Mouse

* Surge protector

The Process
------

All the code I run to set up my cluster can be found in my github.

