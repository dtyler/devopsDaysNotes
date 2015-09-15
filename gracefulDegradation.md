Remote calls != local calls
=========================== 

Increased dependency => increased faults => we need to be mindful of the risk of remote calls

Question: How do we degrade when TimeService fails? (in web app with UserService & TimeService)
Answer:
* Timeouts after 3 seconds
*
*


Timeouts
--------
* Timeouts are often easy to implement
* Switches to failover treatment once timeout is reached
* Applies load to unhealthy server


Circuit Breaker Pattern
----------------------- 
Allows single service to fail without taking down entire system.
* 3 States
   * Closed - All requests go through
   * Open - All requests blocked
   * Half-open - allow one request to test service
* After max fails ciruit breaker transitions to Open
* After reset_time ciruit breaker transitions to Half-open
    * Remain in this loop until request start succeding again
* Benefits
    * fail fast
    * reduces load
* Risks
    * flapping - service goes down each time ciruit breaker closes
    * Pick params based on real metrix for best results

Refernce
danriti/???
