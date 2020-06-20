# MMD - Modular Monolith Design

MMD or Modular Monolith Design is an approach to develop modular monolith applications in a sistematic way. It's based on consolidated backgrounds like Domain Driven Design (http://dddcommunity.org), Enterprise Application Architecture Patterns (https://martinfowler.com/articles/enterprisePatterns.html), SOLID and Object Oriented principles. More than just declaring itself based on Domain Driven Design, MMD proposes to be a more prescriptive DDD specialization in even more specific scenarios.

## Motivations

Since the beggining of 2010's, a new software architectural style became hype: Microservices. Since then, monoliths have been left out, as if they were 2nd class citizens. The times have proved that microservices are a powerful approach to provide solutions for specific complex scenarios, in which monolithic solutions cannot provide the same results. The truth is that these scenarios are in the minority. For most projects, monoliths remain the most effective, simple and inexpensive solution. In these scenarios, the complexity of microservices is not justified. Even in microservices projects, the starting point for the most of projects is a monolith. In both cases, the construction of a modular monolith is a safe path for projects with long life expectancy and frequent changes. A modular monolith provides a healthy application evolution, without the gradual code degradation. It allows a possible distributed services decomposition, with high cohesion and weakly coupled. This project aims to formalize a sistematic approach to develop modular monoliths. It is based on consolidated backgrounds like Domain Driven Desgin, SOLID, Object Oriented Principles and Patterns of Enterprise Application Architecture. This is not a finished product, but a project under construction. Your participation will be very important in this process and I count on it.

## MMD Application Scenarios

MMD should be applied in projects involved in complex needs. Since MMD and DDD are tightly closed, we could say that MMD could be applied in the same scenarios in which DDD applies. There is a quantitative indicator of DDD applicability in the Vaugh Vernon's red book (https://www.amazon.com/Implementing-Domain-Driven-Design-Vaughn-Vernon/dp/0321834577). The method is available here: https://www.informit.com/articles/article.aspx?p=1944876&seqNum=2. Despite of your project's complexity, MMD'patterns can be isolated applied ever they make sense. Look to the patterns described in this document and their applicability. Use them if you you think it makes sense to your project.
 
## MMD Objectives

The MMD's objectives are listed below:

1. Enable writing code ready to change

Software changes should not impact unrelated parts of the application. MMD  aims to help developers to write high maintenable code.

2. Enable writing high readable code

High readability allows developers to quickly understand application's aspects like business rules, achitectural style. Separation of concerns is fundamental to achieve high readability. MMD aims to enable developers to write high readable code.

3. Reduce application inconsistent state possibilities at business level

4. Standardize the way how things are done and where each business aspect is handled

5. Drive creation of libs to support the approach

## MMD Principles

1. Different business contexts implementations 

## Strategic MMD

### Ubiquitous Language

### Bounded Contexts

#### Context Mappings

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
