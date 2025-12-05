![UmaDB Logo](https://raw.githubusercontent.com/umadb-io/umadb/refs/heads/main/images/UmaDB-brand-figure-torso-and-lettering.png)

# What is UmaDB

[UmaDB](https://github.com/umadb-io/umadb/) is an open-source event store server for Dynamic Consistency Boundaries built with Rust.

UmaDB supports event-driven architectures where consistency rules can adapt dynamically to
business needs, rather than being hardwired into the database.

UmaDB directly implements the [independent specification](https://dcb.events/specification/) for
[Dynamic Consistency Boundaries](https://dcb.events) created by Bastian Waidelich, Sara Pellegrini,
and Paul Grimshaw.

UmaDB stores events in an append-only sequence, indexed by monotonically increasing gapless positions,
and can be tagged for fast, precise filtering.

UmaDB offers:

* **High-performance concurrency** with non-blocking reads and writes
* **Optimistic concurrency control** to prevent simultaneous write conflicts
* **Dynamic business-rule enforcement** via query-driven append conditions
* **Real-time subscriptions** with seamless catch-up and continuous delivery
* **OSI-approved permissive open-source licenses** (MIT and Apache License 2.0) 

UmaDB makes new events fully durable before acknowledgements are returned to clients.
