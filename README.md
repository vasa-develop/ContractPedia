# ContractPedia

---

ContractPedia: An Encyclopedia of 40 Smart Contract Platforms
A Complete List of all Smart Contract supportive Platforms

Code Is Law (source)
The blockchain is changing the world as we know it today.
It solves one of the greatest problems know to the mankind: it removes the need of trust. The way blockchain solves it by creating an unalterable trail of anything that needs trust to operate.
But there is lot of power within this technology. 
The power to extend the above property to create rules that need to be followed as written, where every action leads to some reaction.  In other words, smart contracts.
Today we are going to list 40(and growing) platforms/projects that support/develop smart contracts. If you find anything missing or wrong here then shoot that in the comments. Also, the article will be updated regularly as I study more about these platforms and projects.
Here is the Github link to the repository for this article. You can create a pull request for suggesting changes to this article.
P.S. The purpose of the article is to evaluate the platforms/projects on the basis of the factors that will affect their smart contract functionality, not  their overall features.
Articles like this usually take days to complete. If you like reading this type of content and keep this effort continuing then you can show your appreciation and support by buying me a coffee by donating here or to below address:
               a93e64a691d5aff8f78cd63130cf23b89182d235
Here is a list of 40 smart contract platforms/projects.
1. Ethereum
Pros: 
Turing Complete
Enjoys probably the biggest community of developers
Most supported smart contract platform

Cons: 
Uses solidity, which is not as powerful as compared to today's languages such as C++, C#, python, go etc.  
Can prove to be costly if the contract is not written efficiently.

Smart Contract Language: Solidity
Status: Live
Explanation:  Ethereum is one of the first platforms to introduce the concept of smart contracts in the blockchain, and enjoys the support of biggest developer community. It boasts its turing completeness of smart contract platform. The contract code is executed on the EVM(Ethereum Virtual Machine) by every miner in the ethereum network. It is the most used platform used for blockchain based projects.
The platform is a safe bet, but it is blamed for a lot of hacks which has cost its users millions. Also lack of scalablity of the platform results in low transaction speed; making it unsuitable for today's real-world applications. 
The language used(Solidity) is good enough to make it turing complete but it does lacks in the flexibility which is provided by the languages used today. Some problems like:
Not supporting multi-dimensional arrays(eg. string array) in input parameters and return parameters(Here is a workaround)
Only allowing a small number parameters(only 16) in a contract function. (Causing "stack too deep" error)

The above problems show that the contract language still needs to be developed more to match the flexibility of today's languages.
Also your private variables are not actually private, actually anyone in this world with a blockchain explorer can see your so called private variables. Here is how it is done and how you can prevent it.
Here is a list of 62 issues of solidity.
Learning Resources: CryptoZombies, Solidity Docs, OpenZeppelin
2. Quorum
Pros:
Turing Complete
Adds a feature of sending private transactions between 2 or more parties in the network(by use of constellation) which makes it suitable for enterprises
It reduces gas-price to zero, still keeping the gas-limit, thus enjoying the security features provided by use of gas-limit and simultaneously making the transaction cost(gas-price*gas-limit) 0.

Cons:
Relatively small developer community
Same cons as suffered by ethereum due to Solidity as its smart contract language

Smart Contract Language: Solidity
Status: Live
Explanation: In simple words
It is version of Ethereum smart contract platform which provides free-of-cost transactions and is also capable of executing private transactions between selected parties using constellation.



Constellation: Under the hoodIt maintains 2 ledgers: public and private. Public ledger is altered by public transactions and private ledger is altered(only for the parties involved in the the private transactions) by private transactions.
Quorum ArchitectureAs it is closely related to ethereum(same core platform and language), it inherits almost all of the ethereum's pros and cons as a smart contract platform.
Learning Resources: Quorum Docs, CryptoZombies, Solidity Docs, OpenZeppelin
3. Wanchain
Pros:
Adds user privacy in addition to normal ethereum smart contract platform features
Is capable of cross-chain transactions

Cons:
Same as of Ethereum

Smart Contract Language: Solidity
Status: Live
Explanation: It is a fork of Ethereum, thus it inherits a lot of properties of Ethereum. In addition it provides user privacy. Their main focus is on digitizing the current financial model of world on blockchain.
Wanchain's privacy is achieved through the use of ring signatures, which provide complete anonymity to the signer of a transaction while also providing the receiver with the ability to verify the sender's signature. Additionally, Wanchain offers the option for One Time Addresses (OTA) to provide further anonymity optionality.
Wanchain ArchitectureWanchain's distributed ledger builds upon the strengths of Ethereum, and any Ethereum DApp will run on Wanchain without any code alteration. To enhance these applications, Wanchain offers a number of APIs designed to expand cross-chain capabilities and improve privacy protection.
Learning Resources: Smart contracts on Wanchain, Wanchain token, CryptoZombies, Solidity Docs, OpenZeppelin
4. Aeternity
Pros:
Introduced new smart contract language and VMs for faster and safer code execution.
Using State channels and efficient ways to execute contracts keep the transaction prices low.
By providing a version of the EVM it is easy to migrate EVM contracts to Æternity.

Smart Contract Language: Sophia, Solidity, Varna
Status: Live
Explanation: The overreaching functional goal of Æternity smart contracts is to be able to execute code on the chain. That is, code execution that is verified by a miner and which can alter the state of the chain.
The design and implementation of the Æternity smart contracts also have the following non-functional goals in the following order:
Contract execution should be safe.
Contract execution should be efficient and scale.
Contract execution should be cheap.
There should be a simple way to migrate from Ethereum smart contracts.

Goal 1: Contract execution should be safe
With safe contracts we mean that you can specify and automatically prove properties of your contract.
In order to achieve this we have designed a new functional language Sophia and a new safe virtual machine FTWVM.
Goal 2: Contract execution should be efficient and scale
In order to achieve a scalable solution Æternity provides State Channels and a new consensus algorithm.
To get efficient contract execution Æternity provides a very high level language for blindingly fast execution of simple contracts. For more advanced contract the Sophia language can be used. Sophia is compiled to a virtual machine that is tailored for the execution of Sophia contracts. This machine is also high level machine with instructions for operating on the chain and on Sophia data structures without the need to do explicit stack and memory management.
It also uses high-level smart contract language called Varna which is similar to Bitcoin's Script language, but with no loops and a fixed gas price. It uses its own virtual machine - the HLM (High Level Machine) and its code is directly evaluated by the node software. Varna is designed to cover fast, day-to-day contracts.
Goal 3: Contract execution should be cheap
The price of contract execution will ultimately be determined by miners and users, but by providing State channels, efficient ways to execute contracts, and a simple flat rate high level contract language prices should be kept low.
Goal 4. There should be a simple way to migrate from Ethereum smart contracts
By providing a version of the EVM it is easy to migrate EVM contracts to Æternity.
Learning Resources: Smart contract docs, Sophia docs, Sophia Intro
5. Zen
Pros:
Total(see below for explaination) 
As the smart contract language is "Dependently Typed", thus it is less prone to errors and is expressive enough to use it for 'Formal Verification'(see below)

Smart Contract Language: F*
Status: Live
Explanation: Zen Protocol has a very different way of doing smart contracts to other projects.



Zen: I'm differentWe'll start by defining what smart contracts are. In the most abstract sense, a smart contract is a computer program that is designed to run in a decentralized environment - that is, the program is run to determine the consensus of a blockchain. In Bitcoin, smart contracts in the form of Bitcoin Scripts determine whether a transaction is valid or not. In Ethereum, smart contracts in the form of EVM bytecode alter the state of the EVM.
Bitcoin Script is limited in that it is not 'Turing Complete' - it is not possible to express arbitrary computer programs. If we want to express arbitrary logic in smart contracts, then we must be able to have that arbitrary logic evaluated to determine consensus. Turing Complete languages are capable of expressing programs that do not 'halt' - that is, they do not ever finish executing - and it's not possible in general to know if a program finishes terminating, or how long it might take to terminate, or how much computational resources are needed in order to execute the program. Because we don't know how much resources will be needed to execute a program, we can't have Turing Complete languages determine consensus - a program might not halt, meaning that consensus cannot be determined.
Ethereum's EVM is much more expressive than Bitcoin Script. The EVM associates a "Gas Cost" to each EVM bytecode instruction. A user pays a certain amount of "Gas", and the EVM begins to evaluate a smart contract's instructions; It evaluates the gas cost of an instruction, and if there is enough gas to continue, it subtracts the gas cost from the gas that the user has paid for, evaluates the instruction, and continues, failing if it runs out of gas before the execution of it's instructions is complete. In this manner, it's possible to express almost arbitrary computation - Ethereum smart contracts are only limited in that they must terminate eventually, because the user cannot pay infinite gas in order to perform infinitely looping computations. In practice, we are rarely interested in programs that do not terminate, so this restriction is fine.
The EVM's process of interpreting bytecode instructions and tracking gas is very inefficient. For each instruction, the EVM must look up it's gas cost, check that there is enough gas remaining, and subtract the gas cost from the gas remaining. It is difficult to perform optimisations to improve run time with this kind of evaluation model.
The restriction that all smart contracts in Ethereum must be terminating is of interest. Languages in which every program must terminate are not actually Turing Complete - they are 'Total'. Zen uses a total language to express it's smart contracts, rather than relying on an evaluation model that tracks gas in order to ensure totality. Total languages are absolutely capable of expressing arbitrary logic like loops and recursion, and this is the case for Zen Protocol as well.
Zen's smart contracting language is 'Dependently Typed', meaning that every expression has a type, and types may depend on both expressions and types. Dependent type systems are expressive enough to use them for 'Formal Verification' - these types can express arbitrary properties of expressions. For example, whilst in a simply typed language one could give the number 3 the type "Integer", in a dependently typed language, one could also give it the type of "Prime Integer", or "Integer that is less than 10". Dependently typed languages can express resource consumption of programs, which is explained in this blog post.
A typed language will fail to compile if the types are incorrect, and a dependently typed language is no different. A program that expresses incorrect resource consumption or incorrect assertions will fail to compile.
Zen Protocol's smart contract paradigm takes advantage of this. It  takes dependently typed source code, which must express it's resource consumption. If this code compiles successfully, then it's guarantee about resource consumption must be correct, and since we use a total language, we know that it will terminate. Since we know the resource costs from the code itself, we don't need to interpret bytecode instructions and count gas consumption as we go; we know the cost before we run the code. This gives us all of the efficiency benefits of compiled code, as opposed to interpreted code. We currently extract to F#, and compile the F# to CIL bytecode, which we later execute - but it would be possible for other implementations of the Zen Protocol to do this differently, extracting to OCaml or C, for example.
This compilation step only happens once; once code is compiled, it can be executed several times with a huge increase in efficiency.
To lay out the process clearly: A user submits their smart contract source code in a transaction. A node then compiles the code, extracting from it both the program and an expression for it's resource cost. The node can then execute this contract much faster than a node can execute interpreted code. The source code itself is part of consensus; the compiled binaries are not, and only exist locally for the node. Contracts have a delay between being submitted and being "active", allowing nodes to compile contracts in parallel after they receive them, so that they are available for use in a few blocks, but their compilation does not affect transaction throughput.
Smart contracts in Zen are not just faster to run, but can also be executed in parallel most of the time.
Zen Protocol is less limited by the time taken to run smart contracts, and should be able to process transactions involving smart contracts faster - smart contracts in Zen are not just faster to run, but can also be executed in parallel most of the time.
Zen Protocol does not maintain a full virtual machine like the EVM as part of consensus - contracts are separate from other contracts. This enables us to execute contracts in parallel, as opposed to the single-threaded execution of the EVM. This is also a huge efficiency gain, since modern hardware is capable of high degrees of parallelism. Since our contracts are stateless and functionally pure, there are no race conditions or any barriers to parallel execution. Multiple transactions involving the same smart contract may not be easily parallelised, and may have to be executed in series; however since we are running efficient, compiled code, this is still faster than running equivalent computations on the EVM.
Learning Resources: Zen Medium, Zen Docs

6. Counterparty
Pros:
Ethereum smart contracts on top of Bitcoin network(used for consensus).

Cons:
Same as for Ethereum

Smart Contract Language: Solidity, Serpent
Status: Live
Explanation: Counterparty relies on Bitcoin for its consensus. But it also supports ethereum smart contracts.



Counterparty: Bitcoin with EthereumHere is how it works on a higher level:
You write the smart contract code (using Solidity or Serpent) and compile it to a more compact form (bytecode).
Counterparty will create and broadcast a publish transaction to embed this contract code into the Bitcoin blockchain. This is done in a way that is spendable and doesn't "pollute" the blockchain.
Once published, the smart contract "lives" at an address, which looks like a regular Bitcoin address, but starts with a C .
You can then use Counterparty to create and broadcast an executetransaction to call a specific function or method in the smart contract code.
Once an execution transaction is broadcast and confirmed by a Bitcoin miner, every running Counterparty node will receive this request, and execute that method. As the smart contract code executes, it modifies the contract state, which is stored in the Counterparty database. Since each Counterparty node has the same contract code (guaranteed by Bitcoin) as well as the same EVM code, and the code is all deterministic, these state changes are the same for every node.
Others can also send Counterparty assets to the smart contract, which will store them and can use them in future execute calls. This is useful for things like funding contracts, for instance.
Essentially, we see that the publishing of smart contracts and the command to kick off the execution of a specific function or method in a contract are made as actual transactions on the Bitcoin blockchain. Thus, these two operations are limited by Bitcoin's ~10 minute blocktimes. However, once an execution of smart contract code is kicked off, it generally runs as fast as the node can process it.

How does Bitcoin's 10 minute block time affect the EVM?
After a contract is written, it is "published" to the blockchain, which embeds its data in the blockchain, ensuring that all Counterparty nodes have the same contract code to execute. Once published, a method/function on a contract may then be executed.
Both the publishing operation, as well as any execution operations, are published as a Counterparty transaction (inside a Bitcoin transaction) and thus subject to the block time. However, once a contract executes, it will move from line of code to line of code as quickly as the host computer allows, and individual "steps" within a contract are not subject to block times. Nor is a contract executing another contract (via CALL) subject to the block times, and the called contract method (as well as any methods that it calls, and so on) execute immediately.
Thus, the block time limit is overall rather minor, and only affects the initial publishing and the initial execution of a contract method.
Here is an extensive resource which will answer all your doubts about Counterparty.
Learning Resources: CounterParty smart contract docs
7. Rootstock (RSK)
Pros:
Enables Turing complete smart contracts on top on Bitcoin.

Smart Contract Language: Solidity
Status: Live
Explanation: Rootstock (RSK) is a smart-contract platform that incorporates a Turing Complete Virtual Machine to Bitcoin. It also provides other network enhancements, such as faster transactions and better scalability, features which could also enable new usage scenarios.
RSK is the first open-source smart contract platform with a 2-way peg to Bitcoin that also rewards the Bitcoin miners via merge-mining, allowing them to actively participate in the Smart Contract revolution. RSK goal is to add value and functionality to the Bitcoin ecosystem by enabling smart-contracts, near instant payments and higher-scalability.
Learning Resources: Rootstock
8. RChain
Pros:
Turing Complete
Smart contracts enjoy a number of industry-leading functions such as: Meta-programming, Reactive Data Streams, Pattern Matching. As a result, RChain contracts have programmability.

Smart Contract Language: RHOLang
Explanation: RChain is a project which focuses on scalability by using a multi-threaded blockchain with its own smart contract language. It wants to compete with top projects like Ethereum.
RChain is built up following a couple of minimal requirements:
Dynamic smart contract functionality to allow more use cases to be implemented.
Concurrent execution; Multiple independent smart contracts can operate next to each other.
Computationally non-intensive consensus protocol in order not to waste resources: Casper Protocol.

The Java Virtual Machine (JVM) is the foundation of Rho Virtual Machine (RVM). The RVM Execution Environment can operate multiple RVMs with each running a smart contract concurrently and in a multi-threaded fashion. The concurrent structure allows for independent processes to compose into complex processes without competing for resources. This architecture will enable a multi-chain (multiple blockchains per node) effect where transactions are handled on independently executing VM instances.
Rholang Contracts
Rholang contracts can be used on RChain nodes. Rholang is "process-oriented": all computation is done by means of message passing. Messages are passed via "channels", which are rather like message queues. Note that throughout this article the words "name" and "channel" are used interchangeably. This is because in the rho-calculus (on which Rholang is based) the term name is used, however, because you can send and receive information on names, semantically they are like channels. You can play around with some code using the Rholang web interface.
RChain has recreated ERC20 functionality for Rholang. It's now possible to create your token smart contract and deploy it on RChain. You can find the example on their Github.
Learning Resources: RCHain developer site, RHOLang Tutorial

9. Qtum
Pros:
Serves as an improvement upon Ethereum smart contract platform: scalability, lack of formal verification tooling, and lack of lite mobile solutions using simple payment verification (SPV).

Cons:
By being fully EVM compatible and supporting Solidity contracts Qtum inherits all of Ethereum's smart contract security weaknesses.

Smart Contract Language: Solidity
Status: Live
Explanation: Qtum is a smart contracts platform designed to be Ethereum-compatible while addressing some perceived deficiencies of Ethereum such as scalability, lack of formal verification tooling, and lack of lite mobile solutions using simple payment verification (SPV). Qtum addresses these issues with a different underlying blockchain and consensus algorithm that Qtum believes will enable the platform to provide better support for lightweight mobile and Internet of Things (IoT) applications. The project aspires to become the "public blockchain for business" by bringing its technology to financial services, supply chain management, social media, gaming, and other industries in the future.
Qtum is essentially an Ethereum-based smart contracts system running on top of a Bitcoin-based blockchain using a modified version Blackcoin's Proof of Stake (PoS) implementation for consensus. Qtum has added a custom adaptation layer that maps Ethereum account balances to sets of Bitcoin Unspent Transaction Outputs (UTXOs).
By being fully EVM compatible and supporting Solidity contracts Qtum inherits all of Ethereum's smart contract security weaknesses.
Qtum does plan to extend their smart contracts offering to include an x86 virtual machine that would enable the development of smart contracts in languages such as C++, Java, and Haskell. While this would allow Qtum projects to tap into a wider base of developers and leverage existing tooling, it doesn't specifically address the security issues inherent to Solidity's design.
The Qtum white paper states that it is Qtum's objective to develop a Qtum Smart-Contract Language (QSCL) that is claimed to be "backed by formal verification means." No details are provided other than a reference to an academic paper from one of the white paper authors describing another language, developed by that same author, defining a "cross-organizational collaboration ontology." Given the lack of information available about QSCL, it appears that Qtum has not and is not pursuing this initiative.
Learning Resources: Smart contract development Guide
10. Lisk
Pros:
It provides simplified user experience and platform to easily implement custom generated blockchains for anyone from the individual, to the small business, to large banks.

Cons:
Smart contracts are not deployed on Lisk blockchain(mainchain), but on sidechains. This could become a great barrier to develop secure applications using Lisk due to high costs of maintaining a secure sidechain.

Smart Contract Language: Any language
Status: Live
Explanation: Lisk is not in the smart contract business. Lisk intends to allow interfacing with smart contract systems, such as Ethereum, through virtual machine integration. Let me make this clear. Lisk is not a smart contract system, it is a custom blockchain system. platform in which smart contract execution is an optional add-on service. The Lisk blockchain does not store application code, as is normally done with smart contract platforms, but supports a primitive (but extensible) set of predefined transaction types. Lisk has built their business model around creating a simplified user experience and platform to easily implement custom generated blockchains for anyone from the individual, to the small business, to large banks.
Lisk EcosystemLisk runs every single application on a completely separate, isolated sidechain, responsible for itself. Lisk(mainchain) doesn't employ smart contracts. In Ethereum, you deploy your code to the Ethereum blockchain and it gets executed on top of it as a smart contract. Whereas in Lisk, you're not deploying your code to a blockchain(mainchain), you actually create your own blockchain with your custom logic at the core of the blockchain instead of in a smart contract on top of it. So you can create your own custom transaction types, new data stored in transactions, new logic that happens before/during/after transactions.
Refer to this article to understand the concept of sidechains(mainchains and childchains).
Learning Resources: Lisk Smart contract docs
11. Ark
Smart Contract Language: To be decided
Status: Not Live
Explanation: Ark attempts to create a smart contract platform similar to ethereum. The ARK Virtual Machine integration will allow users to issue ARK Smart Contracts. The only difference is that Ark uses dPoS as its consensus mechanism, which makes its transactions faster.
Learning Resources: ACES Ark to Ethereum Smart Contract service
12. EOS
Pros:
Faster contract execution using WASM.
Zero fee transactions.
Uses C++ as smart contract language, which increases programming flexibility.

Cons:
Still needs a lot of community support to "kill" Ethereum(no offence).

Smart Contract Language: C++, C
Status: Live
Explanation: EOS.IO contracts (aka applications) are deployed to a blockchain as pre-compiled Web Assembly (aka WASM). WASM is compiled from C/C++ using LLVM and clang, which means that you will require knowledge of C/C++ in order to develop your blockchain applications. While it is possible to develop in C, it is recommend to use the EOS.IO C++ API which provides much stronger type safety and is generally easier to read.
Application Structure
EOS.IO applications are designed around event (aka action) handlers that respond to user actions. For example, a user might transfer tokens to another user. This event can be processed and potentially rejected by the sender, the receiver, and the currency application itself. As an application developer you get to decide what actions users can take and which handlers may or must be called in response to those events.
Transactions are fast as it uses dPoS as its consensus mechanism, parallel execution, partial evaluation and other optimizations. It is considered as a good competitor to Ethereum due to its high scalability, zero transaction fee, C++ as smart contract language; but it still lacks in wide adoption which will show the actual pros and cons as a smart contract platform.
Learning Resources: EOS developer docs
13. Neo
Pros:
Supports efficient and cheap(computationally) execution of contracts.

Cons:
Small developer community.

Smart Contract Language: C#, VB.Net, F#, Java, Kotlin, Python; they plan to support C, C++, Golang, Javascript
Status: Live
Explanation: The NEO Smart Contract 2.0 includes the following features: certainty, high performance, and expandability. The contract types include: validation contracts, function contracts, and application contracts.
From the performance point of view, NEO uses the lightweight NeoVM (NEO Virtual Machine) as its intelligent contract execution environment. It starts very fast and takes up a small amount of resources and is suitable for smart contracts such as short procedures. Static compilation and caching of hotspot contracts can be significantly enhanced by JIT (real-time compiler) technology. The instructional setup of the NEO virtual machine provides a series of cryptographic instructions to optimize the execution efficiency of cryptographic algorithms in smart contracts. In addition, data manipulation instructions provide support for arrays and complex data structures directly. All of the above will enhance performance in NEO Smart Contract 2.0.
NEO Smart Contract 2.0 achieves a scalable approach through a combination of high concurrency and dynamic partitioning, combined with its low-coupling design. The low coupling contract procedure is executed in a virtual machine (NEO virtual machine) and communicates with the outside through the interactive service layer. Therefore, the vast majority of upgrades to the smart contract function can be achieved through API of the interactive service layer.
From the language point of view, the difference between NEO Smart Contract 2.0 and Ethereum is more intuitive: unlike the original Solidity language in Ethereum, the NEO smart contract can be used directly by almost any high-level programming language. The first supported languages ​​are C#, VB.Net, F#, Java, and Kotlin. NEO provides compilers and plug-ins for these languages, which are used to compile high-level languages ​​into instruction sets supported by NEO virtual machines. The first compiler is for MSIL (Microsoft intermediate language), so theoretically any .Net language and any language that can be translated into MSIL will be immediately supported.
Spite of all this there is no widespread adoption. 
Learning Resources: Neo smart contracts Docs
14. NXT
Status: Live
Explanation: Nxt smart contracts are not Turing complete, but have used a Turing complete scripting layer to create template smart contracts. Users would select the most appropriate template and adjust the parameters to create their own smart contracts. Nxt believes the smart contracts created from these templates should cover most business applications; be easy to code, and ensure safety in the system.
Learning Resources: Nxt smart contracts
15. Nem
Pros:
Fast and scalable

Cons:
A bit centralized and less transparent(see explanation)

Smart Contract Language: No specific language
Status: Live
Explanation: Scalability is the most critical thing about NEM's decentralized application. While ETH does a maximum of 15 transactions per second, NEM reportedly manages hundreds of transactions per second. The NEM foundation has given security and availability a priority.
NEM's blockchain exposes its functionality through a powerful API interface that can be used with any programming language, not a specific "smart contract" language. What Nem cleverly calls "off-chain contracts" is just code using the NEM API. The person running the code can update that at any time, at will without any interaction with the chain. So existing "contracts" can be changed. Depending on what the code does it may be more or less seamless. You can't change something that that piece of code has done on the chain (say reverse transactions) but you can change that piece of code to do something else from now on without interacting with the chain. So in a sense what NEM is doing is less decentralized and transparent but scales a lot better (at least for now) and is a lot more easy to get things done with.
Learning Resources: Nem smart contracts
16. Waves
Smart Contract Language: RIDEON
Status: Live
Explanation: Waves has taken a carefully-considered approach to the implementation of smart contracts. The rollout of the long-anticipated Waves smart-contracts is divided into two stages. The first one is already coming - non-Turing complete smart contracts were launched on 28 April on testnet. The initial release will allow the community to test non-Turing complete contracts, which will enable various account controls and other functionality. Only when these features have been thoroughly tested and activated on mainnet will fully Turing complete contracts follow.
Non-Turing complete smart contracts will cover the majority of the common use cases. It will be a universal and handy tool for implementing any business tasks you potentially might need - from exchanging tokens hosted on different blockchains to establishing precise mechanisms and terms for controlling a shared budget for your project or enterprise. Besides that, non-Turing complete smart contracts are fully secure: the user simply won't be able to make mistake, so the contract will never be fulfilled incorrectly.
One of the first and likely most immediately popular use cases for Waves smart contracts will be multisignature accounts. Another useful application will be token freezing. This involves sending a token to a user, but ensuring it remains non-transferable and unspendable for a period of time. The most obvious use case for this is as a vesting mechanism or for team/contractor payments after an ICO takes place.
A further application of account controls is balance management. A user might want to make regular monthly payments, but to ensure that their account does not fall below a certain balance. Or they might want to keep a fixed amount of funds in one address and move everything above that to a separate account.
Learning Resources: Waves smart contract docs, smart contract IDE 
17. Stratis
Pros:
Uses widely used .NET framework.
It uses the full tried and tested C# package supplied by Microsoft.

Smart Contract Language: C#
Status: Live
Explanation: The most important aspect of the implementation of Stratis smart contracts is they use "real" .NET, which is to say .NET Core is used to execute them. The Stratis Full Node is also written in C# and the route of execution for both it and and a Stratis smart contract is the same. Stratis smart contracts are not just using the C# syntax, they are using the full tried and tested C# package supplied by Microsoft.
Because smart contracts must execute deterministically, they cannot use all capabilities of the C# language or all the .NET Core libraries. The Stratis smart contracts suite includes a validation tool that checks for any non-deterministic elements in any smart contracts that you write.
They also have introduced the concept of gas which is identical to the concept of gas in ethereum.
Learning Resources: Stratis smart contract Docs
18. Stellar
Pros:
Faster, cheaper and more secure than Ethereum smart contract platform.

Smart Contract Language: No specific language
Status: Live
Explanation: 
Stellar smart contracts (SSC) are much different from Ethereum smart contracts. They are not Turing complete and are implemented as an agreement between multiple parties and enforced by transactions. Below you see a comparison between Stellar and Ethereum. Notice the huge difference in cost and confirmation time. A single transaction on the Stellar network costs only ~$0.0000002!
Source: https://www.stellar.org/blog/using-stellar-for-ico/SSCs can be written in any language the Stellar community provides an API for (JavaScript, Python, Golang, PHP, …). You can find an example of a smart contract in PHP here.
An SSC is expressed as compositions of transactions that are connected and executed using various constraints. The following are examples of constraints that can be considered and implemented when creating SSCs :
Multisignature - What keys are needed to authorize a certain operation? What parties need to agree on a circumstance in order to execute the steps?

Multisignature is the concept requiring signatures of multiple parties to sign transactions stemming from an account. Through signature weights and thresholds, representation of power in signatures is created.
Batching/Atomicity - What operations must all occur together or fail? What must happen in order to force this to fail or pass?

Batching is the concept of including multiple operations in one transaction. Atomicity is the guarantee that given a series of operations, upon submission to the network if one operation fails, all operations in the transaction fails.
Sequence - In what order should a series of transactions be processed? What are the limitations and dependencies?

The concept of sequence is represented on the Stellar Network through sequence number. Utilizing sequence numbers in transaction manipulation, it can be guaranteed that specific transactions do not succeed if an alternative transaction is submitted.
Time Bounds - When can a transaction be processed?

Time bounds are limitations on the time period over which a transaction is valid. Using time bounds enables time periods to be represented in an SSC.
Learning Resources: Stellar smart contract Docs
19. HyperLedger Fabric
Pros:
Highly modular platform which allows you to have high control over its performance, scalability and security.

Cons:
As the contracts are deployed on peers(nodes) rather than on network, one has to deploy the contract code on every node(endorsers) on the network.

Smart Contract Language: GoLang, Nodejs
Status: Live
Explanation: HyperLedger Fabric is one of the many projects in the HyperLedger Umbrella.
Hyperledger Fabric (HLF) likes to call its smart contracts 'chaincode'. HLF is an enterprise permissioned blockchain, built with great flexibility, which makes it very useful for businesses as their business rules change after approximately 7 years. Most other blockchains are not built considering flexibility.
HyperLeger Fabric Chaincode FlowHyperledger Fabric itself was written on Go language, so its smart contracts support this language as well. Benefits? Golang is a very efficient language with a fast compile time.
It has a simple contract structure . The three most important functions are:
PutState: Create new asset or update existing one.
GetState: Retrieve asset.
GetHistoryForKey : Retrieve history of changes.
DelState: 'Delete' asset.

Note on DelState: HLF uses a state database that stores keys and their values. This is different from the sequence of blocks that make up the blockchain. A key and its associated value can be removed from the state database using the DelState function. However, this does not mean that there is an alteration of blocks on the blockchain.
The removal of a key and value would be stored as a transaction on the blockchain just as the prior addition and any modifications were stored as transactions on the blockchain.
The history of a key can be retrieved after the key is deleted. There is a GetHistoryForKey() function that retrieves the history and part of its response is an IsDeleted flag that indicates if the key was deleted. It would be possible to create a key, delete the key, and then create the key again; the GetHistoryForKey() function would track such a case.
Learning Resources: HLF chaincode Docs
20. Corda
Pros:
Tailor-made for financial agreements.

Cons:
Each CorDapp is installed at the level of the individual node, rather than on the network itself.

Smart Contract Language: Java, Kotlin
Status: Live
Explanation:
What is a CorDapp?
CorDapps (Corda Distributed Applications) are distributed applications that run on the Corda platform. The goal of a CorDapp is to allow nodes to reach agreement on updates to the ledger. They achieve this goal by defining flows that Corda node owners can invoke through RPC calls.
Note: Each CorDapp is installed at the level of the individual node, rather than on the network itself.
CorDapp InfrastuctureCorDapps are made up of the following key components:
1. States, defining the facts over which agreement is reached
States:
States represent on-ledger facts.
States are evolved by making the current state as historic and creating an updated state.

Each node has a vault where it stores any relevant states to itself.


2. Contracts, defining what constitutes a valid ledger update
Contract:
A valid transaction must be accepted by the contract of each of its input and output states
Contracts are writte in a JVM programming language e.g. Java or Kotlin
Contract execution is deterministic and its acceptance of a transaction is based on the transaction's contents alone
In cases, where transaction validity depend on some external piece of information, such as an exchange rate. In these cases, an oracle is required.

Oracles:
A fact can be included in a transaction as part of a command, An oracle is a service that will only sign the transaction if the included fact is true

3. Services, providing long-lived utilies within the node
Nodes:
A node is JVM run-time with a unique network idetity running the Corda software
The node has two interfaces with the outside world:
A network layer, for interacting with other nodes
RPC, for interacting with the node's owner



The core elements of the architecture are:
A persistence layer for storing data
A  network interface for interacting with other nodes
An RPC interface for interacting with the node's owner
A service hub for allowing the node's flows to call upon the node's other services
A cordapp interface and provider for extending the node by installing CorDapps

5. Serialisation whitelistes, restricting what types your node will receive off the wire
Writing a CorDapp
CorDapps can be written in either Java, Kotlin, or a combination of the two. Each CorDapp component takes the form of a JVM class that subclasses or implements to a Corda library type:
Flows subclass (FlowLogic)
State implement (ContractState)
Contracts implement (Contract)
Services subclass (SingletonSerializationToken)

Learning Resources: Corda smart contract Docs
21. Neblio
Smart Contract Language: C++, Python, Go, JS, Ruby, .NET, Java, Node.js
Status: Live
Explanation: NTP1(Neblio Token Protocol-1) supports the creation of smart contracts created via a set of rules used in the protocol to direct or restrict the movement of tokens. For example a token issuer can set a fee structure for transactions of that token that direct fees to a certain address. Lockup and Expiration rules can be used to move a token to a predetermined address or used to completely invalidate a token after a certain amount of time or on a certain date. Rules can also be used to generate contracts that restrict the addresses tokens can be transferred to, or the addresses allowed to generate new tokens, if any. The way that multiple smart contract languages is possible, is that built into each node there will be RESTful API server that handles all of the API calls and responses for interacting with the Neblio network and blockchain.
Learning Resources: Nebilo Docs
22. Viacoin
Smart Contract Language: Java
Status: Live
Explanation: Viacoin uses RSK(Rootstock) to enable its smart contract functionality. Smart contracts will be compatible with Ethereum. 
Rootstock is a smart contract platform which has a two-way peg. Rootstock runs a turing complete Virtual machine called Rootstock Virtual Machine (which is also compatible with Ethereum virtual machine) and allows solidity compiled smart contracts to run.
The anticipated release of Viacoin is 0.15.0 core, which will see the implementation of Merkelized Abstract Syntax Trees (MAST). MAST, quite simply, allows for smaller transaction sizes, which facilitates better for smart contracts. This is a key release required for Rootstock (RSK) smart contracts, which will give Viacoin Ethereum-like smart contracts. RSK recently released its first beta for a bitcoin smart contracts platform.
Learning Resources: Github
Viacoin Github | Viacoin Reddit | Viacoin Telegram
23. Cardano
Pros:
Heavily focused on making it easier to provide guarantees that a smart contract behaves as designed without hidden vulnerabilities.

Smart Contract Language: Solidity, Plutus
Status: Live
Explanation: The design of the Cardano Computation Layer (CCL), Cardano's smart contracts platform, is heavily focused on making it easier to provide guarantees that a smart contract behaves as designed without hidden vulnerabilities. The CCL consists of two layers: a formally specified virtual machine and language framework, and formally specified languages that facilitate automated verification of human readable smart contract code.
Cardano Smart contracts and VMsThe lowest layer, called IELE, provides a virtual machine designed to make building formal verification tools easy, and a universal language framework for translating smart contracts from higher-level languages into executable instructions. Research and development of IELE is funded by IOHK and led by UIUC Professor and founder of Runtime Verification, Grigore Rosu. Rosu and team are applying insights from their research on KEVM, a formal semantics in the K framework for the Ethereum Virtual Machine, and KLLVM, a formal semantics in K for LLVM, to build a more secure and efficient virtual machine.
Unlike the EVM, which is a stack-based machine, IELE will be a register-based machine, like LLVM. IELE will have an unbounded number of registers and will also support unbounded integers. Avoiding the use of a bounded stack and not having to worry about stack or arithmetic overflow will make specification and verification of smart contracts significantly easier. Like Ethereum, IELE will use gas to limit resource usage and prevent DoS attacks. This presents some challenges to formal verification that are considered "tricky but manageable" by the research team. IELE leverages the K framework to simplify the development of automated tools that verify smart contracts match specifications. This allows IELE to support smart contracts written in any programming language that has a formal semantics in K.
One such language may be Simon. Briefly described in the Cardano vision paper, Simon is a highly constrained, domain specific transaction language that provides a precisely specified set of basic financial transaction primitives that can be combined to create more complicated contracts with verifiable properties. Not much else has been written about Simon, but it is reportedly inspired by concepts from the paper Composing contracts: an adventure in financial engineering, by Simon Peyton Jones and colleagues.
Simon Peyton Jones is one of the principal designers of Haskell, a statically typed, purely functional language that is often used in applications where runtime bugs have a high cost (it is used to implement Ouroboros). Haskell's design makes it amenable to automated verification tools that can identify and eliminate defects early in the software development process. Another Haskell designer and ACM Fellow, Phil Wadler, is a programming languages advisor to IOHK, so it's no surprise that Cardano's primary high level, general purpose smart contract language, Plutus, incorporates many of the concepts behind Haskell.
Plutus is a statically typed, functional language with a human readable, Haskell-like syntax. Like Haskell, Plutus translates to a simpler language, Plutus Core, that makes formal verification easier. Formal verification tools can help developers to reason about contracts and to prove certain properties about the behavior of the smart contract. These proofs can be a powerful tool to highlight and eliminate the primary sources of contract vulnerabilities such as handling of invalid input, type mismatches, nonobvious unintended code paths, confusion around scope, typos, overflows, etc. For example, a proof of the property that there is no code path in which the owner of a contract can be changed would have prevented vulnerabilities that led to both exploits of the Parity multisig wallet. This specific property is obvious in hindsight; it's entirely possible for important properties to be left out of a formal specifications, allowing vulnerabilities that only becomes obvious after they are exploited. So, while formal verification is a very powerful tool, it is only as effective as the human being(s) ability to cover all bases when creating a specification.
Cardano plans to support other high level languages, including Solidity. However it supports Solidity for "for low assurance applications [and Plutus] for higher assurance applications requiring formal verification." While it's hard to imagine any smart contract writer choosing the low assurance option, support for Solidity will make it easier for Ethereum developers and perhaps some existing contracts to migrate to Cardano. The primary reason for developers and contracts to migrate to Cardano, however, won't be its support for Solidity, but rather its ability to reduce the risk of vulnerabilities that put funds at risk. If IELE, Plutus, and supporting verification tools can enable the development of smart contracts that are demonstrably free of the types of vulnerabilities that plague Solidity code, Cardano could become the platform of choice for deploying contracts that need better security around the funds they control (i.e. all smart contracts)
Learning Resources: Cardano Docs
24. Tezos
Pros:
Facilitates formal verification of on-chain code.

Smart Contract Language: Michelson
Status: Live
Explanation: Tezos plans to greatly improve security with Michelson, a new smart contracting language designed specifically to facilitate formal verification of on-chain code. Unlike Solidity, Michelson is not compiled to anything; it is a low level, stack-based, Turing-complete programming language that is directly interpreted by the Tezos virtual machine. So technically it is more analagous to EVM bytecode than Solidity, however it includes high-level constructs such as maps, sets, lambdas, cryptographic primitives, and contract-specific operations to make it easier for humans to read and write. It is purely functional, strongly typed, and statically type-checked to simplify the construction of correctness proofs and eliminate several types of vulnerabilities that have afflicted Solidity contracts.
A correctness proof is not a universal proof that nothing bad can happen, but a proof that all of the assertions enumerated in a certain specification will be satisfied by the program. So if a developer creates a specification that includes an assertion that only authorized users can change the owner of a contract, then the verifier would catch the Parity multisig vulnerability before it got deployed. However, to be effective, the developer needs to think of the assertion (which is obvious only in retrospect) and include it in the specification before deploying the code and witnessing the attack.
Although there is no substitute for human analysis and reasoning in preventing bugs, formal verification is a powerful, complementary tool that is appropriate in situations where bugs can have catastrophic consequences, such as in airplane software and smart contracts controlling large amounts of assets. The Ethereum community recognizes this and there are multipleprojects investigating the formal verification of smart contracts and the Ethereum virtual machine itself. The Ethereum community is also researching new programming languages such as Bamboo and Viper that are more suitable for formal verification and more constrained such that many vulnerabilities can be discovered by compilers rather than by hackers. Since these languages also compile to EVM code, it would be necessary to formally verify both the high-level code as well as the EVM bytecode produced (and/or the compiler producing the bytecode). In contrast, Michelson is interpreted directly by the Tezos VM so requires only a single correctness proof of the contract code.
Once the Tezos blockchain is launched, Michelson will likely provide a programming environment that enables development of significantly safer smart contracts than Solidity by developers with less than expert-level capability. Currently there are at most only a handful of expert Michelson programmers, and being a new, stack-based language without many of the features programmers are used to, the learning curve may present an adoption hurdle for developers. However, Michelson provides a foundation upon which a higher level, more developer-friendly functional language that facilitates "full stack" formal verification could be developed. There is currently active research and development on the Liquidity programming language, which provides an OCaml-like syntax and transpiles to and from Michelson.
In Ethereum, a number of complementary scaling techniques such as sharding, payment channels, sidechains, and off-chain computation are being investigated. Whereas Tezos recognizes that off-chain mechanisms such as payment channels will be required for micropayments, they believe the best route to a massive on-chain scalability boost lies not in sharding but in recursive SNARK technology. SNARKs can be used to provide cryptographic proof of arbitrarily complex transactions, and recursively to provide a single proof for a block of transaction proofs, enabling a large number of transactions to be quickly validated on cheap hardware. According to Breitman this technology could completely eliminate the need for gas limits and allow users to sync the entire blockchain from genesis in less than one second, thereby making the centralization/throughput tradeoff unnecessary. Two key adoption hurdles are the computational cost to produce the recursive proofs and the requirement for a trusted setup, however recent advances suggest that this approach to massive scaling without centralizing may soon be viable.
Learning Resources: Tezos Michelson Docs
25. DFINITY
Smart Contract Language: Solidity
Status: Not Live
Explanation: DFINITY has labeled itself Ethereum's "crazy sister" to express it's close genetic resemblance to Ethereum, differentiated by its obsession with performance and neuron-inspired governance model. 
The idea is that some contract / dapps might be best suited in an algorithmic governance platform rather than a 'code is law' style platform like Ethereum(debatable). The DFINITY project is currently somewhere between prototype and production; there is no public blockchain on which to deploy smart contracts at the time of writing.
DFINITY's biggest selling point is the Blockchain Nervous System (BNS) and its high performance and scalabilty. But one of the thing which will affect our understanding about smart contracts(as mentioned above) is its on-chain governance. 
DFINITY's on-chain governance mechanism allows for protocol upgrades (and much more) without the need to hardfork the network. This is somewhat similar to the idea of Tezos but DFINITY will use the EVM and solidity, so that any contract that can be deployed on Ethereum can also be deployed on DFINITY.
Those who 'stake' their coins in a 'neuron' are given voting power proportional to their stake. The BNS is the collection of all the neurons in the network. Anyone can submit a proposal to the network and those who are staking their coins can vote on the proposals. A proposal can:
Freeze smart contracts/dapps: The network might want to freeze dapps that are used for criminal activity, etc
Reverse transactions: In an event where a bug is discovered smart contract and millions of dollars are stolen or lost (like theDAO or Parity incident), the network can vote to return these lost funds, all without the need for a hard fork.
Edit smart contract code: Imagine a popular dapp is launched to the network, millions of people use this dapp and a bug is discovered. On the Ethereum network, there is nothing you can do to fix this dapp. All you can do is take the code, fix it and launch an entirely new smart-contract. On DFINITY, you could submit a proposal to the network, and have the bug fixed if the community votes to do so. The only way to edit a smart contract like this on the Ethereum network is to hardfork.
Upgrade the protocol: Imagine if Bitcoin was able to absorb the features of all of the alt-coins that were created after Bitcoin. Instead of creating new currencies for Zcash, Ethereum, etc., What if Bitcoin just added features for private transactions, smart contracts, etc. There would be no need for these other currencies. This is the potential power of DFINITY, since the BNS can upgrade the protocol without the need for a hardfork. The reason Bitcoin can't do this is because 1. People cannot agree on which features to add to bitcoin and 2. It would take a hardfork to add new protocol features such as these ones mentioned. DFINITY solves these problems.

Learning Resources: DFINITY Docs
26. BOSCoin
Smart Contract Language: Web Ontology Language
Status: Not Live
Explanation: Unlike most of the smart contract designs mentioned above, BOSCoin's Trust Contracts are designed with the Web Ontology Language and adopting automata theory, aims to be decidable. Lets have a closer look into these components and how they work together.
Web Ontology Language
OWL stands for Web Ontology Language and is based on the W3C Semantic Web language. Under the BOS Platform Trust Contracts, the OWL component aims to interpret the language structure of the smart contracts including the coding and sentence strings.
The World Wide Web Consortium (W3C), is an international community which develops open standards for the longevity of the World Wide Web to support the Web of data. Part of their work is to create a Semantic Web language aiming to represent rich and complex knowledge about things, groups of things, and relationship between things.
The Semantic Web language has 5 main components:
Linked Data: attributes that the database uses to understand languages i.e. dates and titles and part numbers and chemical properties
Vocabularies: languages broken down into their fundamental definitions (i.e. concepts and relationships)
Query: the tool used to retrieve information from databases
Inference: the reasoner that processes and interprets the set of data gathered (i.e. via rules or amalgamating various data from various sources)
Vertical Applications: W3C's business venture component working with different industries to improve research and development, and collaboration - not relevant to this article.

From the W3C Semantic Web, BOS Platform will be utilizing Web Ontology Language. Ontologies are formalized vocabularies of terms, specifying definitions by describing their relationships with other terms within the ontology. OWL is used as a tool for applications to process information (as opposed to humans processing) allowing the system to interpret the meaning of vocabularies; where the information could be standard text sentences or code. The benefit of using OWL is the ability to feed from the multitude of ontologies included in the OWL repositories.
Timed Automata Language
Timed Automata Language (TAL) is the validating agent in BOS Platform's Trust Contracts providing these smart contracts to be decidable. TAL stems from finite automata under automata theory, and is augmented with a timed component to its functionality - hence it would be wise to first understand what automata theory is. Lucky for us there are various publications on this, and the Stanford University provides a good description:
"[Automaton are] automatic processes carrying out the production of specific processes. … Automata theory deals with the logic of computation with respect to simple machines, referred to as automata. Through automata, computer scientists are able to understand how machines compute functions and solve problems, and more importantly, what it means for a function to be defined as computable or for a question to be described as decidable." - Stanford University.
As mentioned above, finite automata is an extension of automata theory. Finite automata refers to a tool to model the logic of finite data and allows for understanding of the resulting state it will eventuate to. An example of this in practice is provided below modelling an automatic sliding door (diagram of door on the left, state diagram on the right):
Schematic Diagram of Sliding Door from SIPSER, Michael (2006). Introduction to Computer Theory. Tomson Course Technology. USA.State Diagram of Sliding Door from SIPSER, Michael (2006). Introduction to Computer Theory. Tomson Course Technology. USA.In the model, the circles represent the states, the arrow represent the transitions. The far left arrow indicates the start state.
The states of the system (for this example, the sliding door) are either OPEN or CLOSED; and for this particular automatic door the outputs can be provided below:
Tabulated Sliding Door Statesi.e. if the system went through the following events FRONT, REAR, NEITHER, FRONT, BOTH, NEITHER, REAR, NEITHER, the states would transition as below:
States of the Sliding Door exampleTimed automata introduces the system's clock as an input to the automaton. An example of using system clock is presented by a popular example of a lamp which, when the switch is pressed subsequently within a limited period of time, the lamp would dim instead of turning only on or off. The state diagram of this is represented below:
Dimming Lamp State Diagram FEHNKER, Ansgar - COMP4151 - Lecture 11a - Algorithmic Verification. University of New South Wales, AustraliaFrom the above Dimming Lamp State Diagram there are 3 states, Off, Dimmedand Bright. The transitions are initiated by a button switch where, if at off state, a single press of the switch would change the lamp state to Dimmed, and if presses within 1 measurement value (you can think of this as a second in terms of time) of the system's internal clock, the lamp state changes to Bright. A press of the switch either at the Bright state, or after 1 second of the previous button press, the lamp's state would be Off.
OWL + TAL + Blockchain
The combination of OWL and TAL provide the fundamental basis for Trust Contracts. With current smart contracts written in code, the OWL component will interpret the structure of the code strings, whilst TAL will be able to model and confirm the logic of overall smart contract - furthermore the information from where OWL and TAL will be sourced is aimed to be stored on the blockchain.
From this we can ensure Trust Contracts are decidable prior to validation and execution of Trust Contracts - ensuring the system's integrity.
Learning Resources: 
27. Agoras Tauchain
Status: Not live
Explanation: To understand Agoras, we first need to explain the Tau-chain principle. That particular ecosystem is a generalization of many centralized and decentralized peer-to-peer networks including blockchain ventures. It has many different use cases ranging from software development to gaming and even decentralized storage. Agoras is an application running over Tau and offers a smart currency with a strong focus on peer-to-peer contracts.
Agoras focuses on peer-to-peer smart contracts. For corporations, Agoras is a solution worth exploring. Companies often want to keep things private, and the smart contracts designed to accommodate such transactions are sufficient to make that happen. Agoras wants to focus on meaningful smart contracts first and foremost. This means these agreements will always adhere to predetermined settings and requirements, without any surprises for either party.
Learning Resources: Agoras blog
28. Burst
Pros:
Turing complete smart contracts.

Cons:
High smart contract fee.

Smart Contract Implementation: Automated Technologies (C/C++)
Status: Live
Explanation: Burst was the first ever cryptocurrency to implement working, turing complete smart contracts in a live environment in the form of Automated Transactions (AT). Below is the flow: from creating a contract to final state change.
Burst smart contract life cycleDue to some problems Burst couldn't catch up with other platforms. As stated in an interview published on April 4, 2018: 
The main issue that I have with Burst ATs is that every opcode (line of code) that is run by a miner costs 1 burst. This makes running a very simple contract - such as sending burst back from the smart contract itself - cost around 20 Burst. If these costs are brought down to maybe 0.001 burst per opcode, it can be just as good as Ethereum or any other platform once we bring in compilers and such.
Learning Resources: BurstAT wiki
29. iOlite
Pros:
Uses FAE (Fast Adaptation Engine), which is capable of converting natural language or any other desired programming language into smart contract code, thus opening the doors of world of smart contracts to a wider audience.

Status: Live
Explanation: iOlite is a product which focuses on the mass adoption of smart contract technology by providing an easy to use engine which is capable of understanding natural language to be compiled to smart contract code. iOlite is the ideal solution if you don't want to spend time learning, instead just start creating smart contracts.
iOlite use caseiOlite is based on the research done at Stanford University. They invented the FAE (Fast Adaptation Engine), which is capable of converting natural language or any other desired programming language into smart contract code. The FAE is not just straightaway translating your input to code. The FAE depends on contributors (smart contract experts) that are able to define structures containing language expressions. Furthermore, these structures are tied to smart contract code they write. This allows the engine to browse the structures to find the right expression so it can compile the desired smart contract. Whenever a structure is used, a contributor gets iOlite tokens rewarded.
As you can see, iOlite relies on their community to make the FAE successful. The FAE helps them by applying Machine Learning techniques to help it learn and adopt new structures more easily.
iOlite Labs is currently focusing on Ethereum smart contracts with Solidity as there is a massive need.
Travis Byrne from the iOlite team explained which languages can be used to create smart contracts. "What this means is that not only can programmers (in formal languages such as Python, C, JavaScript, etc.) immediately use their existing skills to write smart contracts, but also average people with no programming knowledge whatsoever, can just as easily start developing with natural languages like English. iOlite is dissolving the existing technical learning boundaries for creating smart contracts."
Learning Resources: iOlite Guide
iOlite Reddit | iOlite Github | iOlite Telegram
30. ByteBall
Smart Contract Language: Declarative language
Status: Live
Explanation: DAGs is general have a high throughput and scalablity. But this comes with a cost; it is not possible for DAGs such as Byteball to support smart contracts as capable as of Ethereum's. This is because of its tree like structure. 
Byteball DAY structureIn case of Ethereum and other blockchains, this structure is linear. So, it's you can define the ordering of the transactions. Whereas DAGs do not care much about the ordering; they just care about if the transaction is valid or not(is the transaction conflicting). So, DAGs are good for contracts in which the order in which they(transactions) occur doesn't matter. 
Here is where Byteball is different from other DAGs. It has implemented oracles to solve this problem. What oracles do is that they keep the track of all the transactions and maintain a global order of all the transactions in the network. Thus using oracles it is possible to implement smart contracts which require the exact order in which the transactions occurred.
Also, you don't need to be a developer to understand or compose these contracts, you don't need to trust a developer either. Everybody can easily see what the contract means, just like a regular legal contract.
A smart contract in Byteball looks like this:
Composing a Byteball smart contractThis potentially opens the door of its smart contracts for a wider audience; even further across the developer community to the general public.
Learning Resources: Byteball white paper
Byteball Reddit | Byteball Github | Byteball Telegram
31. XTRABYTES
Smart Contract Language: No Specific Language
Status: Not Live
Explanation: DApp developers will be able to access XTRABYTES' core features and data through its Distributed Command Message API (DICOM API). The latter allows DApp code to be developed in a wide array of programming languages. Hence the term code-agnostic. All that will be needed is the ability to call on the API functions within specific code. This will allow developers from a wide array of fields to jump into coding XTRABYTES DApps quickly.
Learning Resources: Xytrabytes Medium
Xtrabytes Reddit | Xtrabytes Github | Xtrabytes Telegram
32. PolkaDot
Status: Not Live
Explanation: A parachain (parallelizable chain) is a simpler form of blockchain, which attaches to the security provided by a "relay chain" rather than providing its own. The relay chain is called that because it not only lends security to attached parachains, but also provides a guarantee of secure message-passing between them. One key feature of parachains is that the computations they perform are inherently independent. Fully generalized systems of turing-complete smart contracts run into issues in determining which transactions will "collide" with each other, meaning that transactions which could potentially be parallelized are often run in sequence, wasting valuable computation time. Drawing clear boundaries between parachains means that we can execute all of them at once without fear of collision - if we have 10 parachains, we can perform 10 times the work using the same source of security.
Polkadot will support both directly connected and fully sovereign but connectable chains. Parachains, or natively supported blockchains that gain consensus using the greater network's consensus mechanism, benefit from Polkadot's pooled security. Pooling security allows each parachain (and the relay chain) to utilize the entire network's set of validators to secure the overall network, meaning each parachain benefits from the network effect of the total ecosystem. If a parachain is compatible with Polkadot, it can leverage the security of Polkadot's consensus mechanism.
Parachain and Bridge ecosystem For other already existing projects with their own state-histories and methods of consensus, Bridges are the connecting layer that will allow them to link to Polkadot. The bridge will connect smart contract-capable blockchains to Polkadot without any modification to their native protocol. Parity Technologies' initial work focuses on bridges connecting two Ethereum-like chains. It can for example transfer value (balances between two chains) from an Ethereum Proof-of-Work (PoW) chain to an Ethereum Proof-of-Authority (PoA) chain and back.
At their core, models like Bitcoin Script and the EVM were designed with the goal of interoperability in mind, but systems making use of these models pay the increased cost of execution for all parts of their implementation, not just those which are meant to be accessible from other systems running on the same network. By contrast, Polkadot parachains communicate with each other by asynchronous message passing, and as such only pay the cost of data uniformity at exactly the boundaries where parachains meet.
Note that it's still possible to create a parachain that provides a framework for fully general, turing-complete smart contracts. A simple example would be a parachain powered by the EVM. Contracts implemented on this parachain would both benefit from and be inconvenienced by the generality and interoperability of Ethereum smart contracts for the reasons given above. The primary difference is that it's fully opt-in. We consider Polkadot's ability to integrate focused solutions while retaining the optionality of using extremely general frameworks to be one of its most powerful features.
Learning Resources: PolkaDot Medium
Polkadot Reddit | Polkadot GitHub | Pokadot Telegram
33. Radix
Smart Contract Language: JavaScript/TypeScript
Status: Not Live
Explanation: Scrypto is a state machine which provides security and functional abstraction to virtual-machines that live on top of it. This enables any VM to interface (providing it can) and execute any script in any language.
The planned JavaScript module will simply be a VM that interacts with the Scrypto state machine.
Learning Resources: Radix developer Intro
Radix Reddit | Radix Github | Radix Telegram
34. Exonum
Smart Contract Language: Rust. Java bindings TBD
Status: Live
Explanation: Services allow specifying the business logic for Exonum applications. They are the main extension points of the framework, which play the same role as smart contracts in some other blockchains.
Exonum Service ArchitectureDeveloping Exonum services is similar to service development in Web or in enterprise platforms; they have the same principal components.
Endpoints
A service has a set of endpoints (realized as REST APIs) using which the service can communicate with the outside world. The Exonum framework acts as middleware, dispatching requests among services and abstracting the intricacies of data (de)serialization, access control, and other typical middleware tasks away from service developers.
There are 3 types of service endpoints:
Transactions correspond to PUT or POST requests in REST
Read requests correspond to GET requests in REST
Private APIs represent administrative and maintenance endpoints, generally not accessible to the outside world.

The key points differentiating Exonum smart contracts from other models used in blockchains are as follows:
Restricted environment. Exonum executes only predefined request types, not allowing to execute untrusted code received from a client. This results in a more controlled environment, and makes it easier to argue about smart contract safety
No isolation. Request processing is performed in the same execution context as the core of the system. This is beneficial for performance, although has certain security risks
Local state. Exonum services may define a local state, which is specific to the node on which the service is running. The local state can be used to manage secret information (e.g., private keys). The local state may be managed by private service endpoints. By utilizing the local state, services can be more proactive than their counterparts in other blockchains. For example, the anchoring service uses the local state to fully automate anchoring transaction signing
Split transaction processing. Transaction verification is a separate step of transaction processing. It is performed immediately after receiving the transaction, before applying the transaction to the blockchain state. Verification may include authentication checks (for example, verifying the transaction signature), as well as other structural checks over the transaction contents. At the same time, transaction verification has no access to the current blockchain state

Learning Resources: Exonum Docs
Exonum GitHub | Exonum Reddit | Exonum Telegram
35. Universa
Smart Contract Language: Javascript
Status: Live
Explanation: To understand how Universa's smart contracts work, we have to break the whole picture into smaller parts.
THE PARTY
Each participant in the Universa is represented by the notion of the party. The party could be completely anonymous or physically identified. There are several ways of identifying a party In the root contract the party could be identified by:
By the public key, mentioned in the contract body (for example, as the issuer or owner).
By the anonymous public key Id which allows identifying the party's public key without disclosing until to the first usage (for example to make anonymous purchases).

The party could add any other details of itself (name, nick, social security or passport number, whatever) in the contract record.
Inside the contract
PARTS
Definition. Immutable part that can't be changed in revisions. Contains issuer, issuing timestamp, permissions (some permissions could be also moved to the state), and any data the creator want to be immutable.
State. The mutable section which could be changed in revisions. Contains revision number, creator and timestamp, reference to the origin and previous revision, changeable roles and (rarely) permissions and any mutable client data.
Attachments. Any file, mentioned by mean of the signed reference in the definition or state.

Universa network knows only definition and state, the rest is never sent to the network. It is important part as attachments may and often contain a sensitive and private information. While this information is well protected by mean of signed references in the contract state and definition, it is even better protected by not being transferred to the Universa network.
So, the full contract is only exchanged between parties involved, where any appropriate transport could be used (email, messengers, clouds, USB flash, whatever). The immutability of the attachments is guaranteed by the signed references in the contract, which are in turn signed by the parties and approved by the network.
So, the chain of trust is:
Universa network approves the revision of the contract, provide the registration time and the immutability of the state and the definition.
Parties that have signed the revision approve (by signing it) that the state and definition are correct, and that they possess all mentioned attachments and agree with them, whatever they are.
Signed references in the state and definition guarantees immutability of the corresponding attachments located somewhere in the client storage.

SCRIPTS
The smart contract could not be smart enough without it. Universa smart contracts allow Javascript to be included as an attachments. The script can implement actions to be performed by clients, generate new contracts, and process events in a completely automated way. The 3rd generation of the Universa client will be able to run as even as an autonomous web service or web application and, in the GUI client, work as a simple GUI application to perform workflow automation together with user interface. Our target is to allow smart contracts to be full-sized application, with all benefits of Universa platform and services incorporated.
Other languages which compile to pure javascript, like Coffeescript, could also be used and even incorporated in the contract as another attachments, but at the execution time only the signed set of compiled javascript will be used.
The scripts are executed by the client software and in the client's environment. The Universa network does not ever see the script, but it always check the result to conform with the contract definition and state. It means, that even if a script will perform some forbidden operation, the network will not accept the result. Generally, it is always simpler to specify few permissions and conditions limiting the allowed operations than trying to check the script source for hidden vulnerabilities. The permissions DSL is clean and straightforward, comparing to the script, and permission check performed remotely by the Universa can not be bypassed by the script, which works locally and is never even transferred to the Universa nodes.
The usual script execution cycle is: scripts is being activated by the user or, in the server environment, some event, like incoming contract or payment notification from our Bitcoin integration service. The script then execute, modify its state (each script have some local storage to work with and can access its contract chain), create and approve with Universa new revisions and derived contracts, and, if need, send it over the network using any connected communication tools. Actually the script could be allowed to connect to any network service using HTTPS API.
Representation
Smart contract is a tree (structure or hash) of objects and could be stored in any modern format, such as JSON, YAML, XML, BOSS, whatever else that can hold arrays, structures, strings and numbers. YAML-based DSL representation is often used as new contract templates, inside the network contracts are always serialized with BOSS, as it is the best to keep binary data that are widely used in Universa (keys, signatures and binary IDs).
THE CAPSULE
Each smart contract is packed to the heavily protected signed container - the capsule. The capsule consist of the body and set of extended signatures. The body includes a packed binary contract itself and set of extended signatures. Each extended signature signs the body and the own type, fingerprint and timestamp, so many types of electronic signatures could be used at once. The corresponding public keys (or it's anonymous IDs) are normally mentioned in the contract body so the system can check whether the mentioned key was used to sign the contract.
The contract's capsule contains no encrypted data, as the part of the contract known to the Universa network should not include any sensitive private data. Instead, such a data must be attached to the contract as signed references (to external files, for example) and will never be transferred to the Universa network, both reducing the unnecessary traffic and protecting private information.
Learning Resources: Universa Docs
Universa Reddit | Universa GitHub | Universa Telegram
36. Urbit
Smart Contract Language: Hoon
Status: Live
Explanation: Urbit is a secure peer-to-peer network of personal servers, built on a clean-slate system software stack. It uses Ethereum for its functioning.
One simple way to think about Urbit is as a "personal blockchain." Like a blockchain, Urbit is a deterministic virtual computer. Its semantics are defined by a frozen lifecycle function, which maps its event history to its current state. But, unlike a blockchain, an Urbit instance is a private computer for one user, not a public record for everyone.
Urbit's lifecycle function is a nano-interpreter called Nock. A typed functional language, Hoon, compiles itself to Nock. An event-driven OS, Arvo, is written in Hoon. Everything above Nock can upgrade itself over Urbit's own overlay packet network, Ames. Ames is live and stable with test keys.
Our Urbit interpreter runs on any Unix machine. The Urbit server is a single-level store - both database and application engine. Every Urbit event is a transaction. Urbit is semantically frozen and cannot call out to Unix.
Your Urbit instance is your personal server. Your urbit should eventually contain and manage your whole digital life. You may compute at home or in the cloud, based on your security/privacy tradeoff, but Urbit's formal semantics makes ships trivial to migrate. You'll never be locked in to one computing provider.
Learning Resources: Urbit Docs
Urbit GitHub | Urbit Reddit | Urbit Telegram
37. Soil
Pros:
Same as of Ethereum

Cons:
Same as of Ethereum

Smart Contract Language: Solidity
Status: Live
Explanation: SOILcoin is an Ethereum-parallel cryptocurrency, using smart contracts and distributed applications (dApps) run over a "global computer network" secured by blockchain technology utilizing the Dagger algorithm. This "Ethereum Virtual Machine" (EVM) is fueled by the digital currency called SOIL, which acts as the gas that runs the computational processes on the SOILcoin network, and is minted through Proof of Work mining.
Learning Resources: Soil Docs
38. Expanse
Pros:
Same as of Ethereum

Cons:
Same as of Ethereum

Smart Contract Language: Solidity
Status: Live
Explanation: It is regarded as first stable fork of Ethereum and its smart contract implementation is same as of Ethereum.
Learning Resources: CryptoZombies, Solidity Docs, OpenZeppelin
39. Ubiq
Pros:
Same as of Ethereum

Cons:
Same as of Ethereum

Smart Contract Language: Solidity
Status: Live
Explanation: Ubiq is a fork of Ethereum with some improvements, but those alterations don't effect much on it's smart contract implementation.
Learning Resources: CryptoZombies, Solidity Docs, OpenZeppelin
40. Ethereum Classic
Pros:
Same as of Ethereum

Cons:
Same as of Ethereum

Smart Contract Language: Solidity
Status: Live
Explanation: It is a fork of Ethereum and its smart contract implementation is same as of Ethereum.
Learning Resources: CryptoZombies, Solidity Docs, OpenZeppelin


---

Other Platforms
Monax , OmniLayer, Ardor
That's all. If you find anything missing or wrong here then shoot that in the comments.
Thanks for reading;)
Articles like this usually take days to complete. If you like reading this type of content and keep this effort continuing then you can show your appreciation and support by buying me a coffee by donating here or to below address:
               a93e64a691d5aff8f78cd63130cf23b89182d235


---

About the Author
Vaibhav Saini is a Co-Founder of TowardsBlockchain, an MIT Cambridge Innovation Center startup.
He works as Senior blockchain developer and has worked on several blockchain platforms including Ethereum, Quorum, EOS, Nano, Hashgraph, IOTA.
He is currently a sophomore at IIT Delhi.
Learned something? Press and hold the 👏 to say "thanks!" and help others find this article.
Hold down the clap button if you liked the content! It helps me gain exposure .
Want to learn more? Checkout my previous articles.
ConsensusPedia: An Encyclopedia of 30 Consensus Algorithms
A complete list of all consensus algorithms.hackernoon.com
Difference between SideChains and State Channels
A complete comparison of the two scaling methods.hackernoon.com
EOS 101: Getting started with EOS, Part 1
The only blockchain which has blocktime of less than a second: 0.5 sec!hackernoon.com
5 resources to get started with ethereum
Ultimate guide for understanding & starting with ethereum.hackernoon.com
Clap 50 times and follow me on Twitter: @vasa_develop
