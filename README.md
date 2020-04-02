# WebAssembly for Blockchain Community Group

This repository with its PRs and issues is used to coordinate work on the WebAssembly components common for the blockchain projects that use WebAssembly.


## Goals

We focus on the components and the discussions that are useful for all WebAssembly-enabled blockchains. That said, components and discussions that are specific to individual blockchains are not part of this vision. From the practical standpoint the goals are:
* Avoiding duplciation of the effort when multiple blockchains work on the same or similar WebAssembly-related problems;
* Have a shared responsibility for security-critical components that we all work together on.

## Common Topics

* Performance of WebAssembly -- something every WebAssembly-enabled blockchain can get behind. We want Wasm code to be executed fast whether using compiler or interpreter. We also want preparation stage, including compilation, injections, static checks to be fast, too;
* Safety of WebAssembly -- the pursuit of performance should not come at a cost of safety. Optimizations to things like gas injection, or optimizations to the Wasm backend should not be violating the safety by allowing to circumvent gas metering or enabling compiler bombs;
* Economic fairness -- many blockchains have only scratched the surface by figuring out how to deduct the fees for the running contract. Figuring out the right fees model that is independent on the platform and not abusable is a common topic for all blockchains;
* Guidelines -- the blockchains have common preferences on what WebAssembly runtime fits which use case, when to use optimizing vs non-optimizing compiler, when to use interpreter, etc. Organizing and maintainign a matrix for runtimes and backends is part of what this group is doing.

## Organization
The CG is a single team that has periodic synchronization events during which they discuss the above topics in pursuit of the above goals:
* Making sure WebAssembly-enabled blockchains are working on common WebAssembly tools together;
* Communicating the needs of the blockchain to other WebAssembly communities and organizations;
* Driving and moderating the recurrent meetings.
