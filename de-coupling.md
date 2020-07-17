# (De)Coupling

* Low coupling as a goal in programming and not only (Unix pipes, etc.)
  * highlight tendency; we spot decoupling tendencies at various levels
  * list advantages
  * list disadvantages
* All direct calls create some sort of coupling, thus yielding systems that are rigid and brittle
* Ways to achieve low coupling
  * basic language/OOP/functional style constructs (don't forget to check Yegor's opinion)
  * design patterns
  * events
  * messaging
  * streaming
  * reactive (?)
  * pipes (?)
* Event-based systems allow a high degree of decoupling (at the expense of traceability)
* Also, one of the tenets of microservices
* Also, DDD
* Also, JAMstack
* So, it's not that we're artificially associating trends but rather, we're converging towards the essence
  as we're solving the same problem at different levels of the stack, over and over again
* Such an architecture poses (new) problems up-front that seem to evolve faster
* Ultimately, think of Unix
