Show a steady progression towards smaller virtual machines

Virtual machines largely kicked off cloud computing, back in roughly 1999.

## Virtual Machines

## Huge hardware

arguably if you make a host with 1TB of ram to hold more VMs, you really just wanted smaller vms, but couldn't do that, so made a bigger host to achieve the same.

## Smaller vms with stripped down OSes

Here we start targeting one vm per application

## Containers

Now applications have been broken down into many containers, but the demarcation is still un-natural

## Functions

This is the absolute limit of virtualization, but we lost something in the persistence

So we are bringing object oriented paradigm to lambda functions. More about allowing persistent state, and message passing to other objects, rather than the fact that these are objects.

## Serverless Objects

This, we argue, is the limiting for of the trend towards smaller virtualization. It is not as small as we can go, but in practical terms it is the smallest self sufficient unit. It happens to align well with how programmers make programs in the first place, and attempts a harmony between developer abstraction, and hardware abstraction, settling on the same fundamental unit.

This is a huge removal of middleware and middle people.

## Fault tolerance

Vmwares FT function
