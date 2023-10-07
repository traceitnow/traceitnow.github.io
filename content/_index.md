+++
title = "Trace It Now"
sort_by = "weight"

+++

# Overview

**Trace it now** is remote tracing debugger for distributed systems.

We are going to create the first remote tracing debugger for distributed
systems (think microservices running on kubernetes).

# Problem

The current state of the art of "printf debugging" is extremely costly:
 - Requires source code modifications, which can introduce more bugs.
 - Requires frequent deployment, which is time consuming.
 - It is error prone, as all code changes are.
 - Logs are left behind, costing extra resources.
 - Programmers are only allowed to debug in production as a last resort.

# Solution

Our solution is a tracing debugger that will run remotely alongside your microservices: 
 - It traces the code at runtime on demand, driven by a central user interface.
 - It doesn't require code changes and does not leave logs behind.
 - It can trace the code across services.
 - And in addition, debugging in production is now safe and easy.
