# W3F Grant Proposal

- **Project Name:** Typechain for Polkadot
- **Team Name:** [SuperColony](https://github.com/Supercolony-net)
- **Payment Address:** ERC 20 ADDRESS:
  0xE1B19cE32866cDE87F8f59C7C2C5f90E093A6942
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 1, 2 or 3

## Project Overview :page_facing_up:

### Overview

Nowadays, when technologies are growing faster and faster, we should think about optimizations of different routine processes and making older stuff better. One of these optimizations is to make code typesafe that will be flexible in different situations.
For now, we have a polkadot.js library, but it provides no typesafe code, so it's hard to understand how to interact with a contract and handle transactions without reading the ABI which becomes challenging. So Typechain is a solution. Developer just need to import the library and use generate typesafe code from contract ABI's.

### Project Details

Typechain reads ABIs of multiple contracts and generates typesafe typescript code, to interact with them. Users can work with on-chain contracts, but also they can deploy the new contract. Typechain will be written on typescript, so it will have CLI to install it and use it multiple times, and also will have the ability to be imported as a package. It will have different arguments, which can configure the generation of contracts. It also will have documentation on how to use it tool, and how to configure it.


The example of usage:

In your project install this package like so:

```bash
npm i -D @supercolony-net/ink-abi-to-ts
```

Now you can use it to generate TS definitions & runtime code for your ABIs.

Given, that you've put input files in `path/to/input` folder, and want generated code to land in `path/to/output` folder, run the following command:

```bash
npx @supercolony-net/ink-abi-to-ts --in path/to/input --out path/to/output
```

### Ecosystem Fit
Help us locate your project in the Polkadot/Substrate/Kusama landscape and what problems it tries to solve by answering each of these questions:

#### Where and how does your project fit into the ecosystem?
Our project can be used by everybody who wants to fasten the development. So it will be a great fit for the Polkadot ecosystem.

#### Who is your target audience

Our main target audience is front-end developers, but it can be also used by other blockchain developers for testing their contracts.

### What need(s) does your project meet?

Our project is a tool that will fasten the development process of Polkadot/Substrate/Kusama projects. It will help you to generate typesafe code from ABIs, and it will also help you to interact with contracts.

### Are there any other projects similar to yours in the Substrate / Polkadot / Kusama ecosystem?

No, we are the first project in the ecosystem. But in Solidity ecosystem there is simmilar projects for example [Typechain](https://www.npmjs.com/package/typechain)

## Team :busts_in_silhouette:

### Team members

- Markian Ivanichok (СEO of Supercolony)
- Toma Sadova (Product Owner | Supercolony)
- Green Baneling (Blockchain Core Rust Engineer | Supercolony)
- Alex Seleznov (Front-End Developer | Supercolony)
- Varex Silver (Blockchain developer | Supercolony)

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
Product Owner
Toma is a Product Owner of OpenBrush, Head of Education and the main organizer of the [the biggest WASM conference](https://wasm-conference.com/). Toma started her career when she was 14. Since then, Toma has gained a lot of experience in IT technologies, management, leadership and crypto. She switched 4 career paths and figured out that blockchain/crypto is her calling!

**Green Baneling**
Blockchain Core Developer
Primary programming languages are: C++, Go, Rust

Finished the faculty of applied mathematics(Master degree). Participated in programming competitions during education. Has worked as a programmer for around 6 years.

Was a freelancer the first year, creating an application for IOS(Swift), creating modules for the desktop application on C++. After that, spent 2 years in a company which created software for TV devices(C++/ Haxe).  After which, for 3 years, worked on different blockchain projects(C++/Go/Rust/Solidity/Js).


**Alex Seleznov**
Front-End Developer

// TODO

**Varex Silver**

Blockchain Developer

Student of Computer Science at the Kyiv National University of Taras Shevchenko. Participated in programming competitions of different stages in school since 2017 (C++).
Was a Backend developer(Go), Solidity developer(Solidity, Hardhat, Typescript), and now Blockchain developer(Rust, Typescript).

### Team Code Repos

- https://github.com/Supercolony-net
- https://github.com/Supercolony-net/<project_1>

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

We have already started working on Typechain, and you can see the progress on our [GitHub repository TODO](TODO)

## Development Roadmap :nut_and_bolt:

### Overview

**We are describing a full roadmap of an TypeChainPolkadot here, with estimates.**

* **Total Estimated Duration:** 10 - 16 weeks
* **Full-Time Equivalent (FTE):** 2
* **Total Costs:** ? USD


### Current work - Scope of this Grant

#### Milestone 1 - Parsing of ABI files

* **Estimated duration:** 2 - 4 weeks
* **FTE:**  1.5
* **Costs:** ? USD

| Number | Deliverable | Specification |
| -----  | ----------- | ------------- |
| 1 | ABI versions support | We will support parsing of ABI v3. Earlier versions are up to a research. |
| 2 | TS types | We will research & match types from ABI to TS types, compatible with [polkadot{.js} v8](https://polkadot.js.org) library. Separately, for methods' arguments and return values. |
| 3 | Parser output | Parsing results in data structure, serving as a base for code generation. |


#### Milestone 2 - Generation of output structure in TS (yet, without methods’ implementation)

* **Estimated duration:** 3 - 4 weeks
* **FTE:**  1.15
* **Costs:** ? USD

| Number | Deliverable | Specification |
| -----  | ----------- | ------------- |
| 1a | Arguments and return values | Generation of TS types definitions for contracts' methods' arguments and return values. |
| 1b | Methods | Generation of methods for `query`, `buildExtrinsic`, `tx` and `methods` namespaces. Without implementation yet. |
| 1c | Contracts' classes | Generation of contract's classes. For both ABIs in `*.json` & `*.contract` input files.
| 2 | Code usability | We will provide JSDoc for generated code, refactor type system for better usability, if needed. |


#### Milestone 3. Methods implementation

* **Estimated Duration:** 4 - 6 weeks
* **FTE:**  1.25
* **Costs:** ? USD

| Number | Deliverable | Specification |
| -----  | ----------- | ------------- |
| 1a | RPC calls | Implementation for the methods, making RPC query calls. |
| 1b | Transactions | Implementation for the methods, related to making transactions. |
| 2 | Contracts deployment | Implementation for the contracts deployment means. |
| 3 | Testing | We will provide tests for correctness of TS type definitions, based on a PSP22 contract. |


#### Milestone 4. NPM packaging & release

* **Estimated Duration:** 1 - 2 weeks
* **FTE:**  1.25
* **Costs:** ? USD

| Number | Deliverable | Specification |
| -----  | ----------- | ------------- |
| 1a | Preparation | We will prepare code for usage as an NPM package with CLI, make sure it works across platforms. |
| 1b | Publishing | Publishing to the [NPM repository](https://npmjs.com). We will provide package's set-up and usage instructions. |
| 2 | Usage examples | We will provide a separate repository with package's usage examples. |


<!-- ### Future work -->



## Future Plans

After this grant, we will be maintaining the project to keep up with new emerging ecosystem standards and also listen to issues from community and update the tool to make the process of transformation a nicer experience for the developers and teams.


## Additional Information :heavy_plus_sign:

How did you hear about the Grants Program?
- Personal recommendation