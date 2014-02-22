> \noindent *"Man is a Tool-using Animal. Weak in himself, and of small stature, he stands
> on a basis, at most for the flattest-soled, of some half-square foot,
> insecurely enough; has to straddle out his legs, lest the very wind supplant
> him. Feeblest of bipeds! Three quintals are a crushing load for him; the
> steer of the meadow tosses him aloft, like a waste rag. Nevertheless he can use
> Tools; can devise Tools: with these the granite mountain melts into light dust
> before him; he kneads glowing iron, as if it were soft paste; seas are his
> smooth highway, winds and fire his unwearying steeds. Nowhere do you find him
> without Tools; without Tools he is nothing, with Tools he is all."*
> \medskip \\
>\noindent -Carlyle





#Preface: Urbit

> \noindent A complex system that works is invariably found to have evolved from a
> simple system that worked. The inverse proposition also appears to be true:
> A complex system designed from scratch never works and cannot be made to
> work. You have to start over, beginning with a working simple system.
> \medskip \\
> Gall's Law


Urbit is a general-purpose programming environment designed to execute a purely
functional network operating system and a referentially transparent network
address space.

Urbit consists of four conceptual levels:

At the lowest-level, Urbit reduces to Nock, a stateless virtual machine based
on combinatory logic and defined in 340 bytes. The Nock machine is sealed -
all execution is "pure." Nock's goal is extreme commoditization of computing
semantics.

Nock acts as our functional equivalent of assembly language. Nock is differs
from assembly language in that it’s interpreted, rather than directly executed
by the hardware. It is like assembly language in that everything in Urbit
executes as Nock and most programming in Urbit will be done using higher-level
tools that reduce to Nock.

Hoon is a high-level language which defines itself in Nock. Its self-compiling
kernel, 7000 lines of code, specifies Hoon unambiguously; there is no Hoon
spec. Hoon can be classified as a pure, strict higher-order static
type-inferred functional language, with co/contra/bivariance and genericity.
However, Hoon does not use lambda calculus, unification, or other constructs
from "PL theory." 

Hoon also excels at handling and validating untyped data, a common task on the
Internet. Its syntax is entirely novel and initially quite frightening a
consequence of Hoon having been designed to optimize for actual usability
rather than cosmetic friendliness. A frequent experience amongst Hoon
programmers is writing code that works the first time it successfully compiles.

Arvo is a deterministic functional operating system and network protocol,
written in 5000 lines of Hoon. Arvo features a revision control filesystem and
the network is a blocking global immutable namespace. Meaning that all data on
the network or off it can be treated as a constant. Additionally, Arvo
preserves a log of all the events it sees, meaning that all computation on an
Arvo instance is recorded and can be played back and examined. 

The network blah blah blah
