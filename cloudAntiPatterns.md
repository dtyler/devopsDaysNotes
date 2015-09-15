Cloud Anti Pattern
=================
1. Finding the sweet spot: combination of CI, CD, and microservices. (platform as a service)
    * Many companies do not look for a combined tool to cover each of these concerns
1. Logic Leak / Service Collision: 
    * Similar logic shared between microservices > inconsient user expirence 
        * SOLUTION: be DRY and merge similiar microservices
1. Monolithic microservices
    * Grouping similiar microservices in same container
        * Issues:
            * Scalling
            * unable to deploy changes rapidly
            * monolithic creep
        * SOLUTION: ONE service per container
    * Premature decompsition
        * issues
            * Do not be in a hurry go micro
        * SOLUTION: Allow natural/gradual migration
1. Ignoring the 3 Musketeers
    * API
        * microservices need to be able to talk to each other
        * SOLUTION: Use swagger.io to keep doc costs low
    * Service discovery/registry
        * microservices need to know about each other
        * SOLUTION: Use tool like Eureka
    * Fault Tolerance
        * Microservices need to by able to tolerate failures (and gracefully degrade)
        * SOLUTION: Use a circut breaker tool like Hystrix
1. Siloed Search
    * Users cannot perform serach across unified data view
        * search data is stale
    * SOLUTION: Federated search model
        * Uses Rabbit or Kafka
        * Search tool listens in a keeps cache fresh

Words
-----
* microservices - software arch design pattern: breaking down a large app > small, independent. One small task done well
* container - isolated and lightweight env for running an applicaiton indendent of an OS

