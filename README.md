![voting](https://user-images.githubusercontent.com/87182167/134034743-229d65be-f64c-41fc-8cb4-e2f0389129f1.png)
# Kubernettes
# Kubernetes (K8s)

[![GoPkg Widget]][GoPkg] [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/569/badge)](https://bestpractices.coreinfrastructure.org/projects/569)

<img src="https://github.com/kubernetes/kubernetes/raw/master/logo/logo.png" width="100">

----

Kubernetes, also known as K8s, is an open source system for managing [containerized applications]
across multiple hosts. It provides basic mechanisms for deployment, maintenance,
and scaling of applications.

Kubernetes builds upon a decade and a half of experience at Google running
production workloads at scale using a system called [Borg],
combined with best-of-breed ideas and practices from the community.

Kubernetes is hosted by the Cloud Native Computing Foundation ([CNCF]).
If your company wants to help shape the evolution of
technologies that are container-packaged, dynamically scheduled,
and microservices-oriented, consider joining the CNCF.
For details about who's involved and how Kubernetes plays a role,
read the CNCF [announcement].

----

This is a python based application which is used for accepting a vote
(voting app).This application accepts the vote and passes it to a
temporary db created using redis.From here the data is passed to a
worker application created using .net which anlysises the data and
stores them permananatly in a database created using postgres
From here the results can be seen on an application that is created 
using nodejs and this is called as resulta-app

To do this we will create 5 pod definition files
and 4 service files,2 services of type cluster ip for redis and postgres 
databases 2 services of type loadbalancer for python voting app and 
nodejs result app
