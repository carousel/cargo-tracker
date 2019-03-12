## Cargo domain vocabulary

-   cargo
-   vessel
-   voyage
-   vessol voyage loop
-   route
-   itinerary (proposed)
-   leg
-   shipping
-   clerk
-   intermodal shipping
-   book
-   claim
-   layover time

### Aggregate represents technical issues, but are rooted deep into domain
-   transaction boundaries (e.g. delayed cargos are locked, locked cargos can't be re-routed)
-   distribution boundaries
-   concurrencty boundaries
-   aggeregates are guide for techical decisions
### Messaging
-   eventual consistency update mechanism


### The routing service will returned connected itenirary

### Internal (existing notes)

### Application

    This is the application layer: code that's needed for the application to performs its tasks. 
    It defines, or is defined by, use cases. It is thin in terms of knowledge of domain business 
    logic, although it may be large in terms of lines of code. It coordinates the domain layer 
    objects to perform the actual tasks. 1This layer is suitable for spanning transactions, security checks 
    and high-level logging.
### Domain

    The domain model, services and repository interfaces. This is the central part of the application. The 
    ubiquitous language is used in classes, interfaces and method signatures, and every concept in here is 
    familiar to a expert in the cargo shiping domain.There is no infrastructure or user interface related 
    code here, except for things like transactional and security metadata which is likely to be relevant 
    to a domain expert ("Either all of foo succeeds or none of it does", "In order to do bar you need to 
    be a Supervisor", and so on).


