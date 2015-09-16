DevOps Operations Challenges
============================
DevOps evolves from frustration
    * lack of communicaiton
    * lack of collaberation
    * poor tooling

DevOps is not
    * a methodology
    * a tool
    * a process

DevOps is
    * a culture
    * a mindset (with a goal of stablizing technology delivery via effective collaberation)
    * breaking down barriers between teams
    * Encourages
        * collaberation
        * communication
        * accountablity
        * faster delivery
        * continuous improvement

Traditional Ops
    * IT infrastructure used to a service published to the rest of the org
    * All request/changes made by ops team
VS
DevOps
    * process becomes more democratized and collaberative

How to start DevOps
    * Functional managers define work and share information on best practices 
    * Challenges
        * Ownership wars
            * Is devops crushing operations?
                * Ops (eg, DBA, networking) no longer has complete ownership 
        * Ops pulled in at the end without understanding
        * "There's an app for that"
            * Ops needs to handle non-ops pushing tools that are not production ready/production quality
        * Legacy meets cloud
            * Many companies use hybrid -> new features in cloud, with legacy non-cloud 
            * monitoring tools need to handle cloud
        * Testing
            * Contact testing
            * microservices testing [link ???]
            * BDD
                * cuucumber ->  specs as tests
        * Time & Budget
            * Training/hiring for new skill sets
            * Costs shfiting from on prem to cloud
                * finance resists non-fixed costs of cloud infrastructure
        * Gloabl teams
            * timezones cause issues with communication
            * solutions 
                * All steps to deiver should be autoamted (CD?)
                * test every change
                * using staging environemt
                * deploy frequently
                * Test in production using feature flags and limited rollouts

My thoughts
-----------
* Team need new resources to handle new requirements of owning more of app lifecycle (CTCT still has "Dev" teams)
* Move to CD works best when it comes from the teams.
