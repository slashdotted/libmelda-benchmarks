# What is Melda?

[Melda](https://github.com/slashdotted/libmelda) is a Delta-State JSON CRDT. CRDTs, which stand for Conflict-free Replicated Data Types, are data structures which can be replicated (copied) across multiple computers in a network. Each replica can be individually and concurrently updated without the need for central coordination or synchronization. Updates made on each replica can be merged at any time.

There exist different types of CRDTs: operation-based CRDTs (which generate and exchange update operations between replicas), state-based CRDTS (which exchange and merge the full state of each replica) and delta-state CRDT, such as Melda, (which exchange only the differences between versions, or states, of the data type).

Melda natively supports the JSON data format and provides a way to synchronize changes made to arbitrary JSON documents. You can work with Melda CRDTs either using this Rust library or using a [command line tool](https://github.com/slashdotted/libmelda-tools/). In the [Kibi w/Melda](https://github.com/slashdotted/kibi) repository you can find a fork of the original [Kibi](https://github.com/ilai-deutel/kibi) text editor with collaboration features implemented using Melda.

In this repository you can find some benchmarks comparing [Melda](https://github.com/slashdotted/libmelda) with [Automerge](https://github.com/automerge/automerge).

# Library and example integration

You can download [Melda](https://github.com/slashdotted/libmelda) from the [main repository](https://github.com/slashdotted/libmelda). In the [Kibi](https://github.com/slashdotted/kibi) repository you will find an example of integration of Melda into a text-editor. There is also another project [libmelda-tools](https://github.com/slashdotted/libmelda-tools/) which implements a simple command line tool to update, read, and meld Melda structures.

# Publications

## 2022
Amos Brocco "Melda: A General Purpose Delta State JSON CRDT". 9th Workshop on Principles and Practice of Consistency for Distributed Data (PaPoC'22). April 2022. (Accepted)

## 2021
Amos Brocco "Delta-State JSON CRDT: Putting Collaboration on Solid Ground". (Brief announcement). 23rd International Symposium on Stabilization, Safety, and Security of Distributed Systems (SSS 2021). November 2021. 

# License
(c)2021-2022 Amos Brocco,
GPL v3 (for now... but I will evaluate a change of license - to something like BSD3/MIT/... in the near future)
