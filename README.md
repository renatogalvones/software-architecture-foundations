# Software Architecture Foundations

My notes about Linked Learning Course [Software Architecture Foundations](https://www.linkedin.com/learning/software-architecture-foundations/microkernel-plugin-architecture)



## Good Architecture
 - Simplicity
 - Maintainbility
 - Testability
 - Focused on the users not in the technology
 
 ## Domain Driven Design (DDD)
  - Ubiquitous language
  - Bounded Context
  
 ### Create Stories
  - Never technical
  - Vertical narrowing (fluxogram)
  - Workflow isolation
  - Identify agents in the system
  - Event storming
  - Define entities
  
 ### Design Patterns
 #### Monolyth
  - Strengths
  - - Homogeneous structure
  - Challenges
  - - Homogeneous structure
 
 #### Plug in <-> Microkernel
  - Strengths
  - - Isolation prevents big ball of mud dependencies
  - - Plugins are small and easy to write, debug, maintain
  - Challenges
  - - Problems within a kernel can bring the system down
  - - Plugins are indirectly coupled through the kernel

#### Message-based
 - Strengths
 - - More maintanable than monolith
 - - Solve dependency problems in microkernel systems
 - Challenges
 - - Managing a highly complex system
 - - Can be very slow and time consuming
 - - Messages have to be stored on disks, replicated, backed up, and so on

#### Microservices
 - Requirements
 - - Small (few hundred lines of source code)
 - - Independently deployable
 - - Fully autonomous
 - - Hides implementation details
 - - Distributed
 - - Highly observable
 - - Modeled around business concepts
 - Strengths
 - - Independent services
 - - Changes do not affect the rest of the system
 - - Changes can occur quickly
 - Challenges
 - - Design and runtime complexity
 - - Networks are slow compared to alternatives

#### Reactive
 - Strengths
 - - Decoupling leads to easier maintenance
 - - Add aditional downstream clients as needed
 - - Faster than declarative
