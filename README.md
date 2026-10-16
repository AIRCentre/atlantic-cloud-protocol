# Atlantic Cloud protocol

The Atlantic Cloud is a transatlantic computing network built and operated by AIR Centre
associates. It pools storage, computing and web infrastructure for research across the Atlantic.
Each node keeps control of its own resources. The service itself is described at
[aircentre.org](https://aircentre.org/en/services/atlantic-cloud).

This repository holds the protocol: what a node must do to be part of that network. The AIR
Centre recommends the reference architecture it runs, documented in the reference paper,
[arXiv:2608.20283](https://arxiv.org/abs/2608.20283). Conformance is judged against the
obligations, not the architecture, so a node built differently is not excluded.

Draft at v0.1. The conformance suite, the provenance schema and the governance terms are not yet
written.

## Read in this order

1. [PRINCIPLES.md](PRINCIPLES.md) - the principles the obligations are derived from.
2. [PROTOCOL.md](PROTOCOL.md) - the obligations themselves.

Each clause names the principles it traces to. To dispute a clause, argue about those
principles.

## Terms

These definitions are part of the protocol. PRINCIPLES.md and PROTOCOL.md use them, and changing
one changes the protocol (C10a).

- **Amendment procedure**: the procedure for changing the protocol's rules (C10a, C10d).
- **Assembly**: the governing body of the nodes (C10a).
- **Catalog entry**: a record describing what an object is. Format: [TBD: schema].
- **Cloud**: the federation of all nodes. Where a decision is meant, the text names the assembly.
- **Custody**: holding data and controlling where it is stored and who can access it.
- **Federated**: offered by a node to the other nodes and their users, by the node's choice (C8).
- **Node**: an institution admitted under C7, together with the infrastructure it operates.
- **Object**: a stored data item, such as a file or a dataset entry.
- **Provenance record**: a record of where an object or workload came from and what it was for.
  Format: [TBD: schema].
- **Record**: a catalog entry, provenance record, resource trace or report a node publishes.
- **Registered image**: a container image listed in [TBD: registry].
- **Resource allocated to the cloud** (allocation): storage or compute a node offers to the
  cloud.
- **Sovereignty**: a node's control over its own data, infrastructure and internal governance
  (C9).
- **Technical body**: the body created under C10b for technical matters.
- **User**: a person or system that runs a workload or uses data on a node.
- **Workload**: a compute job run on a node's resources.

## What the protocol assumes

- Each node owns or operates the infrastructure it offers.
- The data served is meant to be found and used by others, so nodes want it cataloged and
  accessible.

## Contributing

Nodes and institutions considering joining propose changes as pull requests. The main branch
accepts changes only through pull requests.

## License

[CC BY 4.0](LICENSE).
