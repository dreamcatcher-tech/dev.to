---
published: false
title: 'Side Effect IO for Blockchains'
cover_image: 'https://raw.githubusercontent.com/dreamcatcher-tech/dev.to/master/blog-posts/side-effects/assets/mixing-droplet.jpg'
description: Description of the article
tags: infosec, privacy, tor, blockchain
series:
canonical_url:
---

_"Mixing the pure with the impure, without making everything impure"_

The work I have been doing lately could largely be described as side effect
management. This is the means by which to introduce external data into the
blockchain based system, in a way that does not corrupt the key blockchain
property of reproducibility. That is to say, being able to rerun blocks thru
different computers and verify that the same answer came out. Side effects are
any external event - something that cannot be reproduced - a simple example is
receiving an email. The converse is required too - being able to use the pure,
clean, secure blockchain based calculations to trigger unreproducible external
events. A simple example of this is sending an email.

So the work is about making something unrepeatable become something repeatable
in a clean way, and to a lesser extent making something repeatable trigger
unrepeatable events.

However during the work I was doing to send internet packets between Amazon and
the browser the amount of code I was writing that was not blockchain related
started to increase. The problem with this is that it is not reusing the code
that is used for the blockchains, and so requires extra work to build and
maintain, while losing the very helpful traceability properties that blockchain
based calculations afford. Traceability becomes especially useful when the
software is executing on remote servers.

This was the trigger for the work, but it is work that would have been required
later anyway.

I have managed to get the underlying system of side effects working in prototype
form, and starting from this morning I will be applying that to the internet
transport ability. I am pleased with how the system is performing, and it meets
my goals of being clean and simple and easy to fault find. An example of why the
fault finding aspect is useful is that if you call me and say that at roughly
10am something weird happened in the app and you can't seem to make it happen
again, we would be able to see the actual interactions the application made and
very quickly be able to reproduce the problem, making fixing it much faster, and
giving you reassurance that we did actually know what is going on, rather than
having to ask you to keep an eye out for it happening again because we can't
notice anything amiss.
