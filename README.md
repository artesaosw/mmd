# MMD - Modular Monolith Design

MMD or Modular Monolith Design is an approach to develop modular monolith applications in a sistematic way. It's based on consolidated backgrounds like Domain Driven Design (http://dddcommunity.org), Enterprise Application Architecture Patterns (https://martinfowler.com/articles/enterprisePatterns.html), SOLID and Object Oriented principles. Nothing in MDD is new, it just defines a more prescritive way to implement DDD in the code level.

## Motivations

Since the beggining of 2010's, a new software architectural style became hype: Microservices. Since then, monoliths have been left out, as if they were 2nd class citizens. The times have proved that microservices are a powerful approach to provide solutions for specific complex scenarios, in which monolithic solutions cannot provide the same results. The truth is that these scenarios are in the minority. For most projects, monoliths remain the most effective, simple and inexpensive solution. In these scenarios, the complexity of microservices is not justified. Even in microservices projects, the starting point for the most of projects is a monolith. In both cases, the construction of a modular monolith is a safe path for projects with long life expectancy and frequent changes. A modular monolith provides a healthy application evolution, without gradual code degradation. It allows a possible future distributed services decomposition, with high cohesion and weakly coupled. This project aims to formalize a sistematic approach to develop modular monoliths. It is based on consolidated backgrounds like Domain Driven Desgin, SOLID, Object Oriented Principles and Patterns of Enterprise Application Architecture. This is not a finished product, but a project under construction. Your participation will be very important in this process and we count on it.

## MMD Application Scenarios

MMD should be applied in projects involved in complex needs. Since MMD and DDD are tightly closed, we could say that MMD could be applied in the same scenarios in which DDD applies. There is a quantitative indicator of DDD applicability in the Vaughn Vernon's red book (https://www.amazon.com/Implementing-Domain-Driven-Design-Vaughn-Vernon/dp/0321834577). The method is available here: https://www.informit.com/articles/article.aspx?p=1944876&seqNum=2. Despite of your project's complexity, MMD'patterns can be isolated applied ever they make sense. Look to the patterns described in this document and their applicability. Use them if you you think it makes sense to your project.
 
## MMD Objectives

1. Enable writing code ready to change

Software changes should not impact unrelated parts of the application. MMD aims to help developers to write high maintenable and low coupled code.

2. Enable writing high readable code

High readability allows developers to quickly understand application's aspects like business rules, achitectural style. Separation of concerns is fundamental to achieve high readability. MMD aims to enable developers to write high readable code.

3. Reduce application inconsistent state possibilities at business level

MMD aims to avoid all application inconsistent states possibilites at business level. 

4. Standardize the way how things are done and where each business aspect is handled

Uniformity in the code organization favors its developers understanding. MMD aims to standardize how the concepts and actions are organized in the code, so developers can easily understand and start working in a MMD project.

## MMD Principles

1. Domain Model isolated from infrastructure aspects

Business code must be clean so that a code reader can identify the business rules there. Since the business aspects are consolidated and isolated from infrastructure aspects, there is only one place in the code to look for errors.

2. Business code should cover the whole ubiquitous language

All relevant business terms and operations should be expressed by a MDD application's business code. If some business aspect is missing from the business code, it is likely to "leak" to outside the boundaries of the business code. Besides that, a business code focused on represent business process and operations (instead of focused only on software features) favors developers to build valuable software features just reusing code already existent.

3. Business Contexts Separations

Different business context's code should not have direct dependencies each other. This way, distinct context implementations can have their own lifecycle and evolve each in time. Low coupling between different business contexts facilitates code evolution with no conflicts between different parts of code.

4. Standard Patterns and Conventions

Code that is written according to standards is more easily understood by people who follow the same standards.

5. Technology Agnostic

MDD (as well as DDD) should be agnostic about technology in order to people who use different technologies can have benefits of using MDD.

## Strategic MMD

In principle, MDD follows DDD's recommendations at the strategic level.

## Tatic MMD

### Writing Model

#### Entities

#### Value Objects

#### Rich Domains (avoiding primitive obsession)

#### Agregates

##### Agregate Roots

#### Domain Events

##### Event Dispatchers

##### Event Listeners

#### Repositories

### Reading Model

#### Data Transfer Objects (DTO's)

#### Data Access Objects (DAO's)

### Architectural Aspects

#### Domain Isolation

#### Independency of Bounded Contexts

### An example of MMD Implementation with Java/Spring
