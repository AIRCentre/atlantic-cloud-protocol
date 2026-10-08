# Atlantic Cloud protocol

The Atlantic Cloud is a transatlantic computing network built and operated by AIR Centre
associates: a shared pool of storage, computing and web infrastructure for research across the
Atlantic, in which each participating node keeps control of its own resources. The service itself
is described at [aircentre.org](https://aircentre.org/en/services/atlantic-cloud).

This repository holds the protocol - what a node owes in order to be part of that network. A
reference architecture exists and is recommended: it is what the AIR Centre runs, and it is
documented in the reference paper, [arXiv:2608.20283](https://arxiv.org/abs/2608.20283).
Conformance is judged against the obligations rather than against the architecture, so a node
built differently is not thereby excluded.

Draft at v0.1. The conformance suite does not exist yet.

## Read in this order

1. [PRINCIPLES.md](PRINCIPLES.md) - the principles the obligations are derived from.
2. [PROTOCOL.md](PROTOCOL.md) - the obligations themselves.

A clause is settled by the principle it traces to, so an argument about a clause belongs in the
principles.

## What the protocol assumes

- Each participant owns or operates the infrastructure it offers.
- The data served is meant to be found and used by others, so cataloging and access are wanted
  rather than resisted.

## Contributing

Changes arrive as pull requests, from members and from institutions considering membership. The
main branch takes pull requests only.

## License

[CC BY 4.0](LICENSE).
