#Introduction: What is a Personal Cloud Computer?

> \noindent Tlon's three rules of platform warfare:  
> \medskip \\
> 1. General-purpose computers beat special-purpose computers.  
> 2. Personal computers beat industrial computers.  
> 3. Cloud computers beat ground computers.  

Urbit is an open-source software stack that runs a Personal Cloud Computer, or
PC2.  

A PC2 is any general-purpose machine, physical or virtual, that operates
natively on the Internet (cloud), and whose operation is sufficiently simple
that it can be understood and controlled by the user (personal). 

The PC2 is general-purpose, in that it can run programs and applications that
perform a wide range of functions. This is contrasted with special-purpose
platforms, such as a pocket calculator or consumer web application, that can
only perform a single function, or limited range of related functions.

The PC2 is personal, in that the ordinary user can understand its operation
without requiring a high degree of specialized technical skill. This is
contrasted with industrial services, such a Linux server, whose computational
semantics are rendered largely opaque by their complexity, even to the
technically skilled.

The PC2 is a cloud computer, in that it intrinsically operates on a network and
blurs the distinction between network and local resources. This is contrasted
with non-network, or ground, computers, such as the early personal computer,
which maintains a sharp distinction between data on its own disk and data on
the network.

The individual user can easily setup and administer a PC2 on their own, run and
write a endless variety of applications, and can not only can access their
programs and data seamlessly from any client, but can serve any kind of content
to all other clients on the network. Meaning that all programs running on a
PC2 can communicate with programs running on different PC2's as easily as they
can communicate with programs on the same PC2. The PC2 is not just a
general-purpose client, it is also a general-purpose server. In other words, a
network of PC2's is, by definition, a general-purpose social network. 

By no means is this concept an idea original to Urbit. Many, many systems
desinged to implement the PC2 have been tried and, without exception, have
failed to do so. These previous attempts have been crippled by their inadequate
solution two fundamental problems: software portability and network identity.

Portable software can be trivially executed with the same semantics on any
general-purpose computer. One can transfer portable from one machine to any
other machine, and expect it to produce the same output. If the two machines
differ in their output, it is easy to see which one is correct and which has an 
an implementation error.

In contrast, unportable sofware must be modified for each platform
it is run on without any expectation of identical semantics on different
platforms and with complex chains of dependency on other software tools and
libraries, also ususally different per platform.

Unportable software drastically increases complexity, making it difficult for
ordinary users to understand and administer their own general-purpose computer
and incentivizing them to use special-purpose applications and services
administered by others. A lack of portability also makes the goal of
indifference to resource locality significantly harder to acheive. 

[Section on Network Identity needs reworking]

Network identity can best be thought of in the context of the classic computer
science problem of Zooko's Triangle, which states:

The address space of any network can be at most two of secure, human-meaningful
and decentralized.

Secure means that it is impractical for any node on the network to impersonate
another, i.e. when any talks to any other node can authenticate that the node
is who they say they are.

Human-meaningful means that addresses on the network present a good user
interface, e.g. a domain name, such as pets.com, is human-meaningful, an IP
address is not.

Decentralized means that addresses and identities on the network are not stored
with and verified by a central party.

Choosing only secure and human-meaningful but not decentralized effectively
turns your network a large distributed server. Consumer web applications that
claim to be social "networks" are, in fact, simply social servers.

Networks that are secure and decentralized, but not human-meaningful present a
poor interface to the user and fail to gain adoption, because long numbers are
difficult to distiguish from one another. 

And sacrificing secure for human-meaningful and decentralized means that the
network is impossible to defend against malicious activity such as spam.

Succinctly, the problem of network identity is: How does one authenticate
another node in the network? And how does one distinguish between a new user
and a returning spammer?

It would not be too broad a mischaracterization to describe Urbit as a system
that implements portable software on a network with strong identity.

Urbit solves the problem of software portability with a stateless virtual
machine called Nock, which can be thought of as a "Maxwell's equations" of
software. The Nock machine is defined in 340 bytes of pseudocode and executes a
pure Turing-complete function. Nock is not the smallest Turing-complete
computational automaton, but is easily one of the smallest practical ones.
Everything implemented in Urbit is built on top of Nock.

Nock is portable to any platform that can run a Nock interpreter, which is all
general-purpose platforms. Since the Nock specification is conunambigs If two
Nock interpreters disagree with one another, it is trivial to determine which
is wrong and which is right.

Urbit solves the problem of network identity by embedding 

[Section on Network Identity needs reworking]


This book is designed for the novice programmer...
