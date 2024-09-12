## TEE-VM

### Overview

Proofcast TEE-VM is a RISC-V runtime environment inside a Trusted Execution Environment (TEE). It enables builders to write Rust code allowing the execution of guest programs inside a RISC-V VM to provide proof of execution. The necessary I/O primitives are provided to facilitate communication with the VM, with access to a public API. 

Proofcast TEE-VM targets fast and ready-to-use TEE devices, enabling builders to write coprocessors for production use today while preserving low gas impact for on-chain validation. By initially working with AWS Nitro, Proofcast TEE-VM will support all the relevant ready-to-use TEE devices in the future (Strongbox, SGX).  

Developers in the space of dAI, dePIN & on-chain gaming can focus on their core code without setups or maintenance overhead of trusted hardware. They choose Proofcast TEE-VM as a plug&play proving solutions with the best performance / security tradeoff.  



### Components

Proofcast TEE-VM includes the following components:

- **Rust Crate**: Equipped with the necessary I/O primitives to allow communication to and from the RISC-V VM.
- **Command-Line Interface (CLI)**: Serves as the user's gateway to the runtime environment, enabling the execution of user code.
- **TEE Runtime Environment**: Responsible for executing user code, returning the output of computations, and providing proof that the computations were executed as intended. While we provide the execution layer, users deploy their own supported TEE. Initially, we support the StrongBox TEE, with plans to support additional TEEs in the future.

 

### Public Good

Proofcast TEE-VM is a public good: it is freely accessible and operates on a permissionless basis. The Rust crate, CLI, and runtime environment will all be published as open-source repositories. This allows the community to freely access the codebase, fostering collaboration and innovation.

