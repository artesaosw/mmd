# MMD - Modular Monolith Design

MMD or Modular Monolith Design is an approach to develop modular monolith applications in a sistematic way. It's based on consolidated backgrounds like Domain Driven Design (http://dddcommunity.org), Enterprise Application Architecture Patterns (https://martinfowler.com/articles/enterprisePatterns.html), SOLID and Object Oriented principles. Anything in MDD is new, it just defines a more prescritive way to implement DDD in the code level.

## MMD Application Scenarios

MMD should be applied in projects involved in complex needs. Since MMD and DDD are tightly closed, we could say that MMD could be applied in the same scenarios in which DDD applies. There is a quantitative indicator of DDD applicability in the Vaugh Vernon's red book (https://www.amazon.com/Implementing-Domain-Driven-Design-Vaughn-Vernon/dp/0321834577). The method is available here: https://www.informit.com/articles/article.aspx?p=1944876&seqNum=2. Despite of your project's complexity, MMD'patterns can be isolated applied ever they make sense. Look to the patterns described in this document and their applicability. Use them if you you think it makes sense to your project.
 
## MMD Objectives

The MMD's objectives are listed below:

1. Enable writing code ready to change

Software changes should not impact unrelated parts of the application. MMD aims to help developers to write high maintenable code.

2. Enable writing high readable code

High readability allows developers to quickly understand application's aspects like business rules, achitectural style. Separation of concerns is fundamental to achieve high readability. MMD aims to enable developers to write high readable code.

3. Reduce application inconsistent state possibilities at business level

MMD aims to avoid all application inconsistent states possibilites at business level. 

4. Standardize the way how things are done and where each business aspect is handled

Uniformity in the organization of the code favors developers understanding. MMD aims to standardize how the actions are organized in a application, so developers can easily understand and start working ina a MMD project.

## MMD Principles

1. Domain Model isolated from infrastructure aspects

Business code must be clean in order to a code reader can identify the business rules there. Since the business aspects are consolidated and isolated from infrastructure aspects, there is only one place in the code to look for errors.

2. Business code should cover the whole ubiquitous language

All relevant business terms and operations should be expressed by a MDD application's business code. If some business aspect is missing from the business code, it is likely to "leak" to outside the boundaries of the business code.

3. Business Contexts Separations

Different business context's code should not have direct dependencies each other. This way, distinct context implementations can have their own lifecycle and evolve each in time.

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
