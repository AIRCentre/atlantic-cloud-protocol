# Atlantic Cloud protocol

This protocol sets obligations, not an architecture. The obligations change only through the
procedure in C10a–C10d. A node may change its technology at any time. A node adopts the
obligations below and builds however it chooses.

Draft at v0.1. [README.md](README.md) lists what is not yet written and defines the
[terms](README.md#terms). Values marked [TBD] are open.

## Clauses

Each clause is an obligation and names the principles it traces to. Label rules are in
[PRINCIPLES.md](PRINCIPLES.md).

- **C1. The protocol is the commitment; the implementation is free. (P3)** A node conforms by
  passing the conformance suite (C6). The software it runs plays no part in the verdict: Ceph and
  MinIO conform equally.

> *Non-normative.* The AIR Centre runs MinIO, PostGIS and OGC services and recommends them.
> Nodes running the same stack can share expertise and operations. Conformance ignores this
> recommendation.

- **C2. The assembly defines the obligations, identically for every node. (P3, P4)** No node sets
  its own record format or schedule. Nodes must publish process-level provenance, per-object
  accounting and resource traces, as defined in [TBD: schema]. The cloud may read what a node
  publishes. It has no right to access a node's systems or data beyond that.

- **C3. Everything is accounted for, without exception. (P5)** Every object in a resource
  allocated to the cloud must have a catalog entry and a provenance record. Every workload must
  name a registered image and the catalog entries of its inputs and outputs. A missing or
  incomplete record is non-conformance. Conformance is judged on the records, never on the
  content.

- **C4. Reporting is obligatory, and so is its schedule. (P4, P5)** Each node's own
  instrumentation produces records automatically. The technical body can read them at any time.
  Each node also submits a report every [TBD: period] covering every resource allocated to the
  cloud, from the start of the allocation to its end.

- **C5. A node offers compute only where it can trace every process. (P5)** A node may offer
  compute to the federation only on hosts where the node can list, trace and attribute every
  process. The node, not the user running the workload, produces the record, because a user with
  full control of a machine can alter or suppress it. Example, not binding: containers qualify; a
  virtual or physical machine where the user has root does not.

- **C6. Conformance is tested, not declared. (P4)** A node is conformant when it passes the
  conformance suite. Any node can rerun the suite and get the same result. An accession team
  helps the joining node prepare. It has at least one person from the joining node and
  [TBD: number] from existing nodes, appointed by [TBD: body]. The suite decides, not the team.

- **C7. Admission has two stages, and the suite decides the second. (P4, P6)** First, the assembly
  judges eligibility against published criteria. Second, a node that passes the suite is added
  to the public member list at [TBD: location]. The list is alphabetical and nobody can veto an
  addition. The assembly may suspend a node for cause, such as a fabricated record the suite
  cannot detect, under [TBD: suspension and reinstatement procedure]. [TBD: whether a node that
  stops publishing leaves automatically, as P4 says, or is suspended.] If tiers are introduced,
  they describe what a node offers. They never rank nodes, change obligations or restrict access
  to another node's holdings.

- **C8. A node works on its own, and the portal is optional. (P1)** Each node is fully usable
  on its own and chooses, dataset by dataset, what to federate. The cloud runs one portal offering
  access, basic visualization and links to each node's federated APIs. The portal does not
  control access for a node's own users. If it goes offline, every node keeps working. The
  only thing a node owes the portal is a machine-readable service description in [TBD: format].

- **C9. Each node keeps its sovereignty. (P2)** Data never leaves the custody of the node that
  holds it. Each node keeps full control of its own internal governance. A node can withdraw
  at any time with [TBD: notice period] and keep operating on its own. [TBD: what happens to its
  federated records and running workloads.]

- **C10a. The assembly decides what only the nodes together can. (P6)** The assembly has one
  representative per node. It decides admission, suspension, the eligibility criteria and the
  amendment procedure, by [TBD: majority], with a quorum of [TBD: quorum].

- **C10b. The assembly creates the bodies it needs. (P6)** It creates a technical body, a
  scientific body and, where the work warrants one, an ethics body. Each node may nominate
  members. Each body elects its chair and reports to the assembly.

- **C10c. The assembly revises the criteria when needed. (P6)** The assembly may revise the
  eligibility criteria at any time. If an applicant fits the cloud's purpose but fails the
  criteria, the assembly must review the criteria. Revisions are published, take effect for every
  node on [TBD: effective date] and are never retroactive.

- **C10d. The amendment procedure is harder to change. (P6)** Changing the amendment procedure
  requires [TBD: two-thirds] of the assembly.

- **C11. Each version is tagged and states its compatibility. (P6)** A protocol version is a tag
  on the published repository. It states which earlier versions it is compatible with and the
  transition period for nodes to catch up. It has its own conformance suite, so a node can check
  its status against any version. Changes are proposed as pull requests; [TBD: who approves and
  merges them].
