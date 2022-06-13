# W3F Grant Proposal

- **Project Name:** [Typechain-Polkadot](https://github.com/Supercolony-net/typechain-polkadot)
- **Team Name:** [SuperColony](https://github.com/Supercolony-net)
- **Payment Address:** ERC 20 ADDRESS:
0xE1B19cE32866cDE87F8f59C7C2C5f90E093A6942
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** (?)


## Project Overview :page_facing_up:

### Overview

Nowadays, when technologies are growing faster and faster, we should think about optimizations of different routine processes and making older stuff better. One of these optimizations is to make code typesafe that will be flexible in different situations.

When a smart contract is being written, front-end developer receives file representation of it in the format called Application Binary Interface (ABI). One ABI per each contract, new ABI for every update of a contract.

Information about how to interact with a contract (methods names, arguments & returns types etc.) is included in this ABI file. It is not quite human-readable, so extraction of that information becomes a challenge. We need to have correct type definitions for each contract in TypeScript.

Interaction with blockchain is done with polkadot.js library, which only has abstract definitions for the contract in use, thus users' code cannot be typesafe. And Typechain-Polkadot can change it.

### Project Details

Typesafe contracts' descriptions can be generated automatically by a script, taking a list of ABIs as an input, giving usable TS type definitions and even runtime code as its output.

Given, that a front-end developer needs to do this with every contracts update, such tool would save a lot of time and prevent mistakes of misusing smart contracts. It is installed as a package with built-in CLI.

When contracts descriptions come both with ABI and source code (`*.contract` files), our tool will provide means for deployment as well.


### Ecosystem Fit

- Where and how does your project fit into the ecosystem?

There is a whole side to every project in the ecosystem - that is the front-end side of contract integration, - that will find use for Typechain-Polkadot during development process.

- Who is your target audience?

Our main target audience is front-end developers of Polkadot projects.

- What need(s) does your project meet?

Our project speeds up front-end integration of Polkadot/Substrate/Kusama contracts. As well as brings type safety to developers code, when dealing with contracts.

- Are there any other projects similar to yours in the Substrate / Polkadot / Kusama ecosystem?

No, we are the first project of the kind in the ecosystem. However, in Solidity ecosystem, a simmilar project already exists: [Typechain](https://www.npmjs.com/package/typechain).


## Team :busts_in_silhouette:

### Team members

- **Markian Ivanichok** (СEO of Supercolony)
- **Toma Sadova** (Product Owner | Supercolony)
- **Green Baneling** (Blockchain Core Rust Engineer | Supercolony)
- **Alex Seleznov** (Front-End Developer | Supercolony)
- **Varex Silver** (Blockchain developer | Supercolony)

### Contact

- **Contact Name:** Toma Sadova
- **Contact Email:** toma.sadova@supercolony.net
- **Website:** [supercolony.net](https://supercolony.net/)

### Legal Structure

- **Registered Address:** The registered office shall be in 16192 Coastal Highway, Lewes, Delaware 19958, County of Sussex, USA.
- **Registered Legal Entity:** SUPERCOLONY CORP.

### Team's experience

**Markian Ivanichok**
CEO of Supercolony, Blockchain entrepreneur, Software Engineer. Started my engineering career back when I was 15. Since then, I developed and got a lot of experience in engineering and leadership. Gained entrepreneur experience by founding a couple of startups. Inspired, co-founded and invested in Sector F, one of the top consulting companies in Ukraine that helps entrepreneurs to move faster. Since the beginning of this year, co-founded and led Supercolony, a Polkadot venture studio that is dedicated to building and creating of Polkadot’s ecosystem.

**Toma Sadova**
Toma is Market Growth Lead, Product Owner of OpenBrush, and the main organizer of the [the biggest WASM conference](https://wasm-conference.com/). Toma started her career when she was 14. Since then, Toma has gained a lot of experience in IT technologies, management, leadership and crypto. She switched 4 career paths and figured out that blockchain/crypto is her calling!

**Green Baneling**
Blockchain Core Developer
Primary programming languages are: C++, Go, Rust

Finished the faculty of applied mathematics(Master degree). Participated in programming competitions during education. Has worked as a programmer for around 6 years.

Was a freelancer the first year, creating an application for IOS(Swift), creating modules for the desktop application on C++. After that, spent 2 years in a company which created software for TV devices(C++/ Haxe). After which, for 3 years, worked on different blockchain projects(C++/Go/Rust/Solidity/Js).

**Alex Seleznov**
Front-End Developer.
Has 5 years of experience in front-end development. Primarily working with React-based applications with Flux state management systems, written in TypeScript. Produced many modular solutions & dealt with NPM packaging. Latest experience is with projects on Polkadot blockchain.

**Varex Silver**
Blockchain Developer.

Student of Computer Science at the Kyiv National University of Taras Shevchenko. Participated in programming competitions of different stages in school since 2017 (C++).
Was a Backend developer(Go), Solidity developer(Solidity, Hardhat, Typescript), and now Blockchain developer(Rust, Typescript).


### Team Code Repos

- https://github.com/Supercolony-net

Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

- https://github.com/xgreenx
- https://github.com/alex-seleznov
- https://github.com/varex83

### Team LinkedIn Profiles (if available)

- https://www.linkedin.com/in/mivanichok/
- https://www.linkedin.com/in/toma-sadova/
- https://www.linkedin.com/in/alexandr-seleznov-04054b5b/
- https://www.linkedin.com/in/bogdan-ogorodniy/

## Development Status :open_book:

[The project](https://github.com/Supercolony-net/typechain-polkadot) is already a work-in-progress.

## Development Roadmap :nut_and_bolt:

### Overview

**We are describing a full roadmap of the TypeChainPolkadot here, with estimates.**

Technical specifications can be found [here](https://github.com/Supercolony-net/typechain-polkadot/blob/master/docs/tech-specs.md).

* **Total Estimated Duration:** 15 weeks
* **Full-Time Equivalent (FTE):** 2
* **Total Costs:** 60,200 USD


### Current work - Scope of this Grant

#### Milestone 1 - Parsing of ABI files

* **Estimated duration:** 4 weeks
* **FTE:**  1.5
* **Costs:** 16,800 USD

| Number | Deliverable | Specification |
| -----  | ----------- | ------------- |
| 1 | ABI versions support | We will support parsing of ABI v3. Earlier versions are up to a research. |
| 2 | TS types | We will research & match types from ABI to TS types, compatible with [polkadot{.js} v8](https://polkadot.js.org) library. Separately, for methods' arguments and return values. |
| 3 | Parser output | Parsing results in data structure, serving as a base for code generation. |


#### Milestone 2 - Generation of output structure in TS (yet, without methods’ implementation)

* **Estimated duration:** 4 weeks
* **FTE:**  1.5
* **Costs:** 16,800 USD

| Number | Deliverable | Specification |
| -----  | ----------- | ------------- |
| 1a | Arguments and return values | Generation of TS types definitions for contracts' methods' arguments and return values. |
| 1b | Methods | Generation of methods for `query`, `buildExtrinsic`, `tx` and `methods` namespaces. Without implementation yet. |
| 1c | Contracts' classes | Generation of contract's classes. For both ABIs in `*.json` & `*.contract` input files.
| 2 | Code usability | We will provide JSDoc for generated code, refactor type system for better usability, if needed. |


#### Milestone 3. Methods implementation

* **Estimated Duration:** 5 weeks
* **FTE:**  1.5
* **Costs:** 21,000 USD

| Number | Deliverable | Specification |
| -----  | ----------- | ------------- |
| 1a | RPC calls | Implementation for the methods, making RPC query calls. |
| 1b | Transactions | Implementation for the methods, related to making transactions. |
| 2 | Contracts deployment | Implementation for the contracts deployment means. |
| 3 | Testing | We will provide integration tests based on a PSP22 contract. Testing will check correctness of generated TS type definitions. |


#### Milestone 4. NPM packaging & release

* **Estimated Duration:** 2 weeks
* **FTE:**  1
* **Costs:** 5,600 USD

| Number | Deliverable | Specification |
| -----  | ----------- | ------------- |
| 1a | Preparation | We will prepare code for usage as an NPM package with CLI, make sure it works across platforms. |
| 1b | Publishing | Publishing to the [NPM repository](https://npmjs.com). We will provide package's set-up and usage instructions. |
| 2 | Usage examples | We will provide a separate repository with package's usage examples. |


<!-- ### Future work -->


## Future Plans

After this grant, we will be maintaining the project to keep up with new emerging ecosystem standards and also listen to issues from community and update the tool to make the process of transformation a nicer experience for the developers and teams.


## Additional Information :heavy_plus_sign:

We haven’t applied for any other grant programs for this project.

**How did you hear about the Grants Program?**

Have a number of approved applications:
- OpenBrush
- Sol2Ink
