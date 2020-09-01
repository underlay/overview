# Underlay

Last updated: Sept. 1st, 2020

## Table of Contents

- [The Underlay](#the-underlay)
- [The Underlay Project](#the-underlay-project)
- [ARC Protocol](#arc-protocol)
- [Collection Server Protocol](#collection-server-protocol)
- [R1 Registry](#r1-registry)

## The Underlay

The Underlay is a distributed knowledge graph. It is an emergent structure that arises from a network, similar to the World Wide Web. 

## The Underlay Project

The Underlay project is a team of people developing protocols and tools that enable the Underlay to exist. The protocols are expected to have a finite lifetime and are designed in a way that pieces of the technical underpinning of the Underlay can grow and adapt over time.

The project currently has three focuses:
- ARC protocol
- Collection Server protocol
- R1 registry

## ARC Protocol

The ARC protocol defines the core data model and schema language for the Underlay. ARC stands for 'Assertions, Reduction, Collections'.

The basic premise is to structure knowledge graphs as a series of positive immutable statements called _assertions_. These transactional assertions are transformed into a singular materialized view through a process called _reduction_. Assertions can be grouped together in _collections_ which define the schema and reduction mechanics. These collections are designed to be published, shared, and integrated into other collections.

The ARC protocol is developed and documented in the [underlay/arc-protocol](https://github.com/underlay/arc-protocol/) repo.

## Collection Server Protocol

The Collection Server Protocol is used to interact with _collection servers_, which host collections and expose interfaces for managing, updating, and querying collections. Collection servers in the Underlay are analogous to file servers on the Web, and can be used locally or remotely.

The Collection Server Protocol is developed and document in the [underlay/collection-server-protocol](https://github.com/underlay/collection-server-protocol) repo.

## R1 Registry

A registry is a hosted instance of a collection server that manages collections and implements usage policies. Registries can implement query capabilities, user authentication, social structures that facilitate collaboration, or other policies the maintainers deem useful. Registries in the Underlay are analogous to websites.

R1 is the name of the first registry being developed by the Underlay project. It is developed in the [underlay/r1](https://github.com/underlay/r1/) repo and accessible at https://r1.underlay.org.
