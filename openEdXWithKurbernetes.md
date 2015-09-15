Open edX with Kurbernetes
=========================

Kurbernetes
-----------
* scheduling and orchestration layer
* abstracts infrastructure
* 1.0 released in July 2015
* Adds healthchecking, secret management, and service discovery (beyond docker utils)

Pods
----
Groups of containers and volumes

Service
-------
* Provides endpoint for pods
* basic load balancing
* Can wrap non-dockerized resources

Replication Controllers
-----------------------
* manages life cycle
* provides scaling + fault tolerance 

Lessons
-------
* Containers should be stateless
* Start up tasks (run once) cause issues
    * SOLUTION: factor these tasks into their own container
