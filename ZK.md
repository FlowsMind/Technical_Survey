# [ zero-knowledge proof ]

01. gnark (https://github.com/ConsenSys/gnark)

`gnark` is a framework to execute (and verify) algorithms in zero-knowledge. It offers a high-level API to easily design circuits and fast implementation of state of the art ZKP schemes. 

`gnark` has not been audited and is provided as-is, use at your own risk. In particular, `gnark` makes no security guarantees such as constant time implementation or side-channel attack resistance.

02. emmy -- Library for zero-knowledge proof based applications (like anonymous credentials) (https://github.com/xlab-si/emmy)

Emmy is a library for building protocols/applications based on zero-knowledge proofs, for example anonymous credentials. Zero-knowledge proofs are client-server protocols (in crypto terms also prover-verifier, where the prover takes on the role of the client, and the verifier takes on the role of the server) where the client proves a knowledge of a secret without actually revealing the secret.

Emmy also implements a communication layer supporting the execution of these protocols. Communication between clients and the server is based on Protobuffers and gRPC. Emmy server is capable of serving (verifying) thousands of clients (provers) concurrently. Currently, the communication is implemented for the two anonymous credential schemes (see Currently offered cryptographic schemes).

03. ZKRP -- Reusable library for creating and verifying zero-knowledge range proofs and set membership proofs. (https://github.com/ing-bank/zkrp)

This repository contains ING's implementations of Bulletproofs, Zero Knowledge Range Proof (ZKRP) and Zero Knowledge Set Membership (ZKSM). The current implementations are based on the following papers:

Range Proofs based on the paper: Efficient Proofs that a Committed Number Lies in an Interval by Fabrice Boudot.
Set Membership Proofs based on the paper: Efficient protocols for set membership and range proofs, by Jan Camenisch, Rafik Chaabouni and Abhi Shelat.
Bulletproofs based on paper: Bulletproofs: Short Proofs for Confidential Transactions and More, by Benedikt Bünz, Jonathan Bootle, Dan Boneh, Andrew Poelstra, Pieter Wuille and Greg Maxwell.
