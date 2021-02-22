There are four main types of tuning that are done on Interblock after every major change. These are listed in order of decreasing difficulty, and decreasing abstraction.

## Protocol Tuning

How the protocol operates, avoiding high level wastage such as requiring 3 blocks to initialize a chain, when 2 is the minimum. Sending interblocks with only promise updates. Sending only diffs in interblocks.

## Architecture tuning

The design for how to operate the protocol, particularly with interactions between databases, processors, and websockets. The architecture was designed to not just implement the protocol, but to use the protocol in its own implementation.

## Implementation tuning

Code level specifics of the implementation of the architecture. eg: how to hash faster, how to stringify faster

## Application tuning

The end application can be modified to use the features of the blockchain to advantage. Mostly this is taking advantage of the near unlimited multithreading ability, by pushing operations out to the edge of the system, rather than controlling from a centre.

It is rare than an application requirement would cause protocol tuning to occur.
