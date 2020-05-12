# Getting started with Cisco Modelling Labs (Personal and Enterprise)

Cisco Modeling Labs is a tool for building virtual network simulations (or labs) for you to test out new topologies, protocols, and config changes; automate network tests via CI/CD pipeline integration; and learn new things about the cool world of networking. Cisco Modelling Labs 2 has been rebuilt from the ground up.

Network simulation is becoming an increasingly important area, particuarly with organisations looking to adopt network automation, we often need safe environments where we can test and understand our automation tooling is working correctly so that when we deploy to production networks we know what we're expecting to happen.

One of the key usecases of CML-2 is for integrating in CICD. One of the advtanges of CML-2 is the new REST API which allows us to automate the creation and running of simulations. After doing an intitial introduction we'll explore the API and understand how it can be leveraged.

# Sandbox environment

To follow this lab you will need an instance of CML2. For this you have 2 options the first to build your own environment or to use the prebuilt DevNet sandbox.

If you are looking to build your own CML environment you'll first need to purchase licenses for  limited to 20 nodes Can be purchased for $199. If you are interested in purchasing CML Personal you can do so from this [link](https://learningnetworkstore.cisco.com/cisco-modeling-labs-personal/cisco-cml-personal) 

There is also a Enterprise edition which allows a higher node count and more flexibility in terms, for more information on this reach out to your Cisco account team or a Cisco partner.

Alternatively, if you'd just like to try CML out you do have the excellent DevNet sandbox where you can reserve an instance of CML2 for up to 4 hours. This sandbox provides access to a Cisco Modeling Labs system that can be used to explore the capabilities of the newest release of Cisco Modeling Labs. This is quite a generous with almost 40GB of RAM and 57GB of disk space so theres space to do some pretty decent simulations. All DevNet sandboxes are completely free and can be accessed within seconds.

https://developer.cisco.com/docs/sandbox/#!overview/all-networking-sandboxes 

# The Basics

If you're using the sandbox when you first login there's already a premade simulation you can try out. I'm going to stop and delete this for now and walk you through the process of creating you're own simulation but feel free to explore the simulation to get to grips .


Cisco Modeling Labs – Today Cisco Modeling Labs supports the following Cisco images:
IOSv and IOSvL2
NX-OSv and NX-OS 9000v
IOS XRv and IOS XRv 9000
IOS XE (CSR1000v)
ASAv


# The API

One of the real advantages of this version of CML is the excellent API which allows us to automate many of the common tasks when using CML. As mentioned previously this could allow for integration into a CICD pipeline. 

Tasks we could automate include:

* Spin up and down simulations
* Edit simulations while running (add extra link, add node etc)
* Get detailed information from devices on a simulation
* Conduct actions such as a packet capture

# Python SDK
