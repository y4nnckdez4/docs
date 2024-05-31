## TEE-VM

### Overview

Proofcast TEE-VM is a RISC-V runtime environment inside a Trusted Execution Environment (TEE). It enables builders to write Rust code allowing the execution of guest programs inside a RISC-V VM to provide proof of execution. The necessary I/O primitives are provided to facilitate communication with the VM, enabling the execution of arbitrary code within our TEE and generating proof of its execution as expected.

Proofcast TEE-VM represents a step forward in cross-chain communication by targeting fast and ready-to-use TEE devices, enabling builders to write coprocessors for production use today while preserving low gas impact for on-chain validation. By initially supporting StrongBox TEE, Proofcast TEE-VM provides an accessible and efficient solution for developers and organizations requiring robust, secure cross-chain interoperability.

Developers can focus on their core code without the costly or slow setups of alternative technologies. By targeting the RISC-V architecture, Proofcast TEE-VM aligns with market standards and remains open to new and optimized solutions in the future.


### Purpose and Use Cases

The primary purpose of Proofcast TEE-VM is to provide builders with a tool for accessing and verifying states across different blockchains. This tool is chain-agnostic, and capable of working with any blockchain, from Ethereum to non-EVM chains.

It addresses several critical issues in cross-chain communication by enhancing seamless interaction between different blockchain networks, improving data management and integration, facilitating the fluidity of assets across platforms, reducing the risk of single points of failure, improving the efficiency of interactions between isolated blockchains, and providing flexible trust models in cross-chain interoperability solutions.


### Competitive advantages

Proofcast TEE-VM provides a modern and efficient solution for cross-chain communication, enabling generic code to be compiled and executed on existing TEEs at a fraction of the time and cost associated with on-chain verification. Key benefits include:

- **Efficiency**: Faster execution and lower on-chain verification costs compared to traditional methods.
- **Compatibility**: Maintains close compatibility with ZKp systems, allowing users to switch between TEE and ZK solutions easily.
- **Scalability**: Supports the creation of a variety of coprocessors for production use with low gas impact for on-chain validation.
- **Accessibility**: Initial support for StrongBox TEE, which is inexpensive and widely available, unlike alternative centralized solutions.


### Components

Proofcast TEE-VM includes the following components:

- **Rust Crate**: Equipped with the necessary I/O primitives to allow communication to and from the RISC-V VM.
- **Command-Line Interface (CLI)**: Serves as the user's gateway to the runtime environment, enabling the execution of user code.
- **TEE Runtime Environment**: Responsible for executing user code, returning the output of computations, and providing proof that the computations were executed as intended. While we provide the execution layer, users deploy their own supported TEE. Initially, we support the StrongBox TEE, with plans to support additional TEEs in the future.


### Industry Context

Proofcast TEE-VM is positioned within the rapidly advancing landscape of coprocessor technologies, influenced by contributions from projects such as Succinct's SP1, RISC Zero, and Jolt. These projects have improved the execution of generic code on RISC-V VMs and enhanced ZK proofing speeds. Despite the promise of ZK systems, they still face significant computational inefficiencies and high on-chain verification costs, which can be a barrier for many builders.

### Public Good

Proofcast TEE-VM is a public good: it is freely accessible and operates on a permissionless basis. The Rust crate, CLI, and runtime environment will all be published as open-source repositories. This allows the community to freely access the codebase, fostering collaboration and innovation.

