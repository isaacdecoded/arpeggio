# ARPEGGIO

Minimalistic but extendable software development template based on Clean Architecture, SOLID principles and DDD approach for Microservices and go on.

## Introduction

In music context, arpeggios are melodic combinations of notes that have in common their belonging to a certain chord or tonality. Said in a slightly easier to understand way, it would be to spread out (place one after the other instead of sounding them all at the same time) the notes of a chord or certain notes of a tonality or scale.

Now imagine each layer of a software architecture as notes and each implementation of these layers as arpeggios, i.e: the execution of a Command (refering to CQRS) is a combination of processes that are implemented from infrastructure layer to domain layer so this Command will combine each layer in order to make a success mutation, an arpeggio.

# Explanation

Lets start by defining the software architecture layers (described as directories) from inner to outer as Clean Architecture dictates:

- Domain: contains the system core definitions as Entities, Domain Events, Repositories and Services interfaces, etc.

- Application: contains all the application business rules as Use Cases, Domain Event Handlers, etc.

- Adapters: contains the intermediates between Infrastructure and Application layer as controllers, presenters, etc.

- Infrastructure: contains all the implementation details about technologies, storage systems, external services integrations, etc.

## Full-layered Implementation
You maintain Infrastructure Layer abstraction as much as possible.

## Framework-based Implementation
You basically forget about Adapters Layer and start implementing external libraries or frameworks.

# Using pre-commit Git Hook

Run ln -s pre-commit .git/hooks/pre-commit

## Conclusion

There are many ways of development, patterns, principles, concepts, preferences, etc., and this template is just another proposal of project organizing that pretends to provide an starting point for good practices and advanced approaches as DDD and SOLID without losing simplicity as contradictory as it sounds.