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

- Where and how does your project fit into the ecosystem?
- Who is your target audience (parachain/dapp/wallet/UI developers, designers, your own user base, some dapp's userbase, yourself)?
- What need(s) does your project meet?
- Are there any other projects similar to yours in the Substrate / Polkadot / Kusama ecosystem?
    - If so, how is your project different?
    - If not, are there similar projects in related ecosystems?

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

This section should break the development roadmap down into milestones and deliverables. To assist you in defining it, we have created a document with examples for some grant categories [here](../docs/grant_guidelines_per_category.md). Since these will be part of the agreement, it helps to describe _the functionality we should expect in as much detail as possible_, plus how we can verify and test that functionality. Whenever milestones are delivered, we refer to this document to ensure that everything has been delivered as expected.

Below we provide an **example roadmap**. In the descriptions, it should be clear how your project is related to Substrate, Kusama or Polkadot. We _recommend_ that teams structure their roadmap as 1 milestone ≈ 1 month.

For each milestone,

- make sure to include a specification of your software. _Treat it as a contract_; the level of detail must be enough to later verify that the software meets the specification.
- include the amount of funding requested _per milestone_.
- include documentation (tutorials, API specifications, architecture diagrams, whatever is appropriate) in each milestone. This ensures that the code can be widely used by the community.
- provide a test suite, comprising unit and integration tests, along with a guide on how to set up and run them.
- commit to providing Dockerfiles for the delivery of your project.
- indicate milestone duration as well as number of full-time employees working on each milestone.
- **Deliverables 0a-0d are mandatory for all milestones**, and deliverable 0e at least for the last one. If you do not intend to deliver one of these, please state a reason in its specification (e.g. Milestone X is research oriented and as such there is no code to test).

> :zap: If any of your deliverables is based on somebody else's work, make sure you work and publish _under the terms of the license_ of the respective project and that you **highlight this fact in your milestone documentation** and in the source code if applicable! **Teams that submit others' work without attributing it will be immediately terminated.**

### Overview

- **Total Estimated Duration:** Duration of the whole project (e.g. 2 months)
- **Full-Time Equivalent (FTE):**  Average number of full-time employees working on the project throughout its duration (see [Wikipedia](https://en.wikipedia.org/wiki/Full-time_equivalent), e.g. 2 FTE)
- **Total Costs:** Requested amount in USD for the whole project (e.g. 12,000 USD). Note that the acceptance criteria and additional benefits vary depending on the [level](../README.md#level_slider-levels) of funding requested. This and the costs for each milestone need to be provided in USD; if the grant is paid out in Bitcoin, the amount will be calculated according to the exchange rate at the time of payment.

### Milestone 1 Example — Implement Substrate Modules

- **Estimated duration:** 1 month
- **FTE:**  2
- **Costs:** 8,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | Apache 2.0 / GPLv3 / MIT / Unlicense |
| 0b. | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can (for example) spin up one of our Substrate nodes and send test transactions, which will show how the new functionality works. |
| 0c. | Testing Guide | Core functions will be fully covered by unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article**/workshop that explains [...] (what was done/achieved as part of the grant). (Content, language and medium should reflect your target audience described above.)
| 1. | Substrate module: X | We will create a Substrate module that will... (Please list the functionality that will be implemented for the first milestone) |  
| 2. | Substrate module: Y | We will create a Substrate module that will... |  
| 3. | Substrate module: Z | We will create a Substrate module that will... |  
| 4. | Substrate chain | Modules X, Y & Z of our custom chain will interact in such a way... (Please describe the deliverable here as detailed as possible) |  


### Milestone 2 Example — Additional features

- **Estimated Duration:** 1 month
- **FTE:**  1
- **Costs:** 4,000 USD

...


## Future Plans

After this grant, we will be maintaining the project to keep up with new emerging ecosystem standards and also listen to issues from community and update the tool to make the process of transformation a nicer experience for the developers and teams.


## Additional Information :heavy_plus_sign:

How did you hear about the Grants Program? 
- Personal recommendation