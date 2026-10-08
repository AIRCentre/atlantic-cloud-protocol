# Atlantic Cloud protocol

The Atlantic Cloud is a protocol, not an architecture. Engineering evolves; the commitment must
not. A participating institution adopts the obligations below and builds however it chooses.

Draft at v0.1. The clauses are stated; the operation sets, the provenance schema and the
governance terms they refer to are not yet written.

## Clauses

Each clause is an obligation. Labels are permanent, on the same terms as the principles above.

- **C1. The protocol is the commitment; the implementation is free.** A node conforms by meeting
  obligations, never by running a named stack. Ceph, or anything else that passes, conforms
  equally.

A common stack is nonetheless recommended rather than merely illustrated. The AIR Centre runs
MinIO, PostGIS and OGC services, and a node running the same shares the expertise, the training
and the operational burden with everyone else who does. Maintaining a cloud is not easy, and that
is worth urging. It is not worth obliging: the recommendation binds nobody, and conformance does
not look at it.

- **C2. The cloud defines the obligations, identically for every node.** No node sets its own
  terms, record format or schedule. What must be published is prescribed and not negotiable, and
  it is deep: process-level provenance, per-object accounting and resource traces are all obliged.
  The one thing the cloud does not take is an unbounded right to go and look - it specifies what a
  node publishes rather than helping itself to the rest.

- **C3. Everything is accounted for, without exception.** An object resolving to no catalog entry
  and no provenance record is non-conformance, as is a workload that cannot bind a registered
  image to cataloged inputs and outputs. What is judged is the account rather than the content:
  abuse surfaces as the inability to produce a conformant record, so nobody reads anyone's data to
  find it.

- **C4. Reporting is obligatory, and so is its schedule.** Records are produced automatically by
  each node's own instrumentation and stand open to the cloud's technical bodies continuously.
  Periodic reports cover every resource allocated to the cloud, for the whole period of the
  allocation.

- **C5. Federated compute runs where the host can enumerate its processes.** The offering node
  traces every process, attributes it, and publishes the record. The record is the node's to
  produce, because capacity whose holder controls its own record produces no record at all. By way
  of illustration, binding nothing: a container runtime leaves processes visible to the host,
  while a machine under its holder's full control does not.

- **C6. Conformance is tested, not declared.** A node is conformant when it passes a suite whose
  result any member can reproduce. Getting there is joint work, done by an accession team from the
  existing and the joining nodes; the verdict stays the suite's.

- **C7. Admission has two stages, and the second is mechanical.** Eligibility is judged against
  published criteria. Admission takes effect only on published conformance, and from passing to
  being listed, alphabetically, there is no discretion. Suspension for cause is the one judgment
  the cloud keeps, because the suite cannot catch a fabricated record. A tier, if one ever
  emerges, describes properties and never standing: it cannot change what a node owes or gate
  access to another node's holdings.

- **C8. Independence precedes federation, and the entry point is additive.** A node is useful
  alone and federates per dataset. The cloud has one visible entry point - access, minimal
  visualization, routing to each node's eligible APIs - which sits over the federation, cannot
  gate a node's own users, and whose absence leaves every node fully usable. What a node owes it
  is a machine-readable service description.

- **C9. Sovereignty is preserved by construction.** No custody moves, no governance is delegated,
  and an institution can withdraw and keep operating.

- **C10. The cloud is governed by an assembly of its member nodes.** The assembly holds what only
  membership can decide - admission, suspension, the eligibility criteria, the procedure for
  changing them - and constitutes the domain bodies it needs: technical, scientific, and ethical
  where the work warrants one. Each is drawn from all nodes and elects its leader. The protocol
  names the functions that must be answerable rather than an org chart. The criteria are revised
  as the world changes, and an applicant who makes sense but does not meet them is a reason to
  look at them again. A revision applies to everyone, stays revised and is published. An applicant
  is judged against published criteria, and the procedure for changing them costs more to change
  than an ordinary decision.

- **C11. Versioned, with compatibility stated.** A node must be able to establish whether it still
  conforms. A version is pinned by a tag on the published repository rather than by a copy of this
  file.
