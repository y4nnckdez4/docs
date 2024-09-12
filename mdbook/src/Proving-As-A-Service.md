# Welcome to the Proofcast Documentation

Visit our [website](https://www.proofcast.xyz/). Stay updated with the latest news by following us on [X](https://www.x.com/proofcastlabs). Builders, developers, and curious minds are welcome to join our [Telegram group](https://t.me/proofcast_builder) to chat with the team.


Proofcast is a products suite that **democratizes access to cryptographic proofs backed by Trusted Execution Environments (TEE) with the first _“proving-as-a-service”_ solution based on trusted hardware.**  

### **What are TEEs?**

TEEs are isolated execution environments within the main processor, where both code and data are protected at the hardware level. The secure enclave ensures:

1. **Confidentiality**: code and data within the TEE are isolated and cannot be accessed by any unauthorized components, including the operating system and hypervisor.
2. **Integrity**: the code and data within the TEE are shielded from tampering, even by privileged software or physical attacks on the hardware.
3. **Hardware Attestation**: TEEs support cryptographic attestation, enabling the generation of verifiable proofs that the code executed inside the TEE is authentic and has not been altered.

### **Why it matters?**

The transition of blockchain infrastructure to a modular design—such as the separation of settlement and execution in Ethereum—has created a demand for **coprocessors**. These are designed to offload on-chain computation to specialized layers optimized for efficiency and cost, enabling data-intensive and computation-heavy applications.

Cryptographic proofs, particularly succinct proofs, have become the standard to ensure the security, integrity, and confidentiality of these off-chain computations


### **The limit of zk-proofs & the future of TEEs**

zkVMs (like SP1 or Risc0) accelerated the adoption of zk-proofs with a revolution in abstraction and user experience, eliminating the need to design custom circuits and reducing overhead for developers.

We believe the same will happen with Trusted Execution Environments. 

The next generation of on-chain applications will rely on the co-processing power provided by TEEs. Use cases like decentralized physical infrastructure networks (dePIN), decentralized AI (dAI), and on-chain gaming cannot be fully supported by zk technology alone.

However, many teams today face the challenge of building trusted hardware solutions from the ground up. They must develop custom applications and code, all while navigating fragmentation between various TEEs (like Intel SGX, AWS Nitro) and diverse proving networks.


### **The future of TEEs: “proving-as-a-service”**

![](./Proving-as-a-service.png)

Proofcast wants to become the “proving-as-a-service” standard for TEEs.

We bet on giving developers better accessibility and UX by leveraging:

- **Abstraction**: working with TEEs should be as simple as pressing a button and running your code;
- **Selection**: our stack aims at supporting all types of devices (Intel, AWS, Android, etc.);
- **Customization**: no lock-in network or standalone product, but a suite tailored to specific needs.

Our go-to-market is a suite of products that currently range from the first general-purpose TEE-VM, to event attestator (cross-chain) and light clients.
