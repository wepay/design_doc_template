# design_doc_template
A generic design document template for documenting Micro services.

# Title

##### Author: **

## Introduction

*What is the goal of the service? What is the problem statement?*

If there are any product specification documents, link them to appendix.

## Potential Solutions

*Section should include alternative implementations/solutions*

*Document all the Spikes done to evaluate potential solutions.*

*Should start documenting what was done prior to the spike, what are the specific problems and what kind of solution do we value.*

*Is it feasible? If the time runs out, “we don’t know yet” is a perfectly acceptable answer to “is it feasible?”. Document what you tried or learned so any other team member could continue if it is decided to resume the spike.*

*How much effort does it need for each approach? Pro’s and con’s of each approach. The goal of a spike would be to produce knowledge, document results and to reduce uncertainty.*

*Document what were your alternatives, why you made the decision and how that will affect (positively and potentially negatively) the team and the project.*

*Knowledge produced and documented as a result of Spike should be enough for the product owner to create the stories to do the real work and help the development team to estimate it.*

## Assumptions

 *Clearly document any assumptions you are making to define clear scope of the deliverable.* 

## Constraints / Limitations

 *List of all the things that this system is NOT intended to do or can not do.* 

## System Design and Architecture 

### System diagram or flowchart 

 *Interaction diagram of various inputs, outputs, sub systems and dependencies.* 

### Terminology and components

*Nobody likes abbreviations, list of all the key terms and abbreviations.*  

### Hard and soft dependencies

 *What will be the impact on the system if these dependencies go down?* 

### Algorithm or Pseudocode for main components

*Describe your logic in this section.*

### Service guarantees that you expect

 *ACID requirements, Fault tolerance and recovery. If something goes wrong, will the service be able to auto recover or the recovery process has to be manual.*  

### **Data definition, schema design and Persistence requirements**

*Describe your data model and entity relationships*

### Caching requirements 

*What are you planning to cache? What will be the size the cache? For how long?* 

### Capacity planning

 *How much data will the service generate, retention policy, and sharding.* 

### Performance requirements 

 *Expected throughput and SLA. How did you came up with these numbers?* 

### Security 

 *Any PII / PCI data being handled by service?* 

### Multi region story

 *Any special requirements your service needs to achieve HA must be listed here. E.g. By default, BigTable doesn’t replicate data across zones or regions. If you are using that to store data, explain how will you handle zone outages.* 

## API / gRPC Endpoints 

[Instructions](https://github.com/pseudomuto/protoc-gen-doc#writing-documentation) for documenting gRPC methods and services 

## Rollout Plan

- Define the roll out phases
- A/B tests that you plan to do as part of the rollout
- Data migration 

## Test Plan

*How are you planning to test the service? How will you test the dependencies? Will you be creating the mocks for dependencies or using a sandbox environment? How are you planning to run load and performance tests?* 

## Appendix 

- References, links to additional documentation (E.g. Product specification or Business requirements with acceptance criteria )

## Review Sign-Off

### Internal Review

- **Team lead/manager**: *Sign-off by* 
- **Sponsor**: *Sign-off by* 

**Target sign-off:** no late than *2 weeks from date of submission - format MM/DD/YYYY (WWW).**



**[Sign-off Completed on]**
