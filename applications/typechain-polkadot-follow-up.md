# W3F Grant Proposal

- **Project Name:** [Typechain-Polkadot](https://github.com/Supercolony-net/typechain-polkadot)
- **Team Name:** [SuperColony](https://github.com/Supercolony-net)
- **Payment Address:** ERC 20 ADDRESS:
  0xE1B19cE32866cDE87F8f59C7C2C5f90E093A6942
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 2


## Project Overview :page_facing_up:

### Overview

This Grant is a follow-up to the previous grant, [W3F Grant Proposal](https://github.com/w3f/Grants-Program/pull/992).
We have decided to add new tool that will help developers to easy integrate typechain to their projects, and it will be also compatible with Redspot (if redspot was used to compiler project, you can just left most of things).
We have some updates in our team, so check it out. And also we made more work on Milestone 1 than we thought, so now it'll be easier to add new features to the project, so we considered to reestimate our time.

### Usage of Typechain-compiler

```bash
    npx typechain-compiler --config config.json
```

Also you can set some additional arguments like `--noCompile`, `--noTypechain`, `--release`

Config interface will be something like this:
```typescript
export interface Config {
    projectFiles: string[]; // Path to all project files, everystring in glob format
    skipLinting : boolean; // Skip linting of project files
    artifactsPath : string; // Path to artifacts folder, where artifacts will be stored it will save both .contract and .json (contract ABI)
    typechainGeneratedPath : string; // Path to typechain generated folder
}
```

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

**Varex Silver**
Blockchain Developer.

Student of Computer Science at the Kyiv National University of Taras Shevchenko. Participated in programming competitions of different stages in school since 2017 (C++).
Was a Backend developer(Go), Solidity developer(Solidity, Hardhat, Typescript), and now Blockchain developer(Rust, Typescript).

**Artem Lech**
Blockchain Developer.

Student of Applied Mathematics at the Kyiv National University of Taras Shevchenko. Started programming from 2016, participated in a lot of Ukrainian and international competitions of competitive programming. Worked as a lecturer of algorithms at school of competitive programming and as Intern Backend Engineer (Rust). Now works as Blockhain Developer on Polkadot Blockchain (Rust, Typescript).

### Team Code Repos

- https://github.com/Supercolony-net

Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

- https://github.com/xgreenx
- https://github.com/varex83
- https://github.com/Artemka374

### Team LinkedIn Profiles (if available)

- https://www.linkedin.com/in/mivanichok/
- https://www.linkedin.com/in/toma-sadova/
- https://www.linkedin.com/in/bogdan-ogorodniy/
- https://www.linkedin.com/in/artem-fomiuk-31249b226/

## Development Status :open_book:

[The project](https://github.com/Supercolony-net/typechain-polkadot) is already a work-in-progress.


## Development Roadmap :nut_and_bolt:

### Overview

### Current work - Scope of this Grant

#### Milestone 2 - Full coverage for ABIs’ types. Contracts deployment.

* **Estimated duration:** 4 weeks
* **FTE:**  2
* **Costs:** 44,800 USD

| Number | Deliverable | Specification |
| ------ | ----------- | ------------- |
| 0a | License | MIT |
| 0b | Documentation | We will cover new-added features in documentation and usage examples. |
| 1 | Investigation | Broaden types definitions for methods arguments and return values (to full coverage). |
| 2 | Parser & generators modules | Design and implement a new parser module for ABI JSON to work with different versions of the ABI. Parser's output structure serves as an input for generators. Refactor, replace inlne generation with parser to generator flow. |
| 3 | Contract deployment | Support of parsing `*.contract` files. Provide means for contract deployment. |
| 4 | Testing | Full coverage of PSP22 contract with integration tests. Both for contract usage and deployment. We will be testing arguments' & return values' types correctness. |


#### Milestone 3 - Optimization. Improve type system of the generated code.

* **Estimated duration:** 4 weeks
* **FTE:**  2
* **Costs:** (was 33,600, now ???) USD

| Number | Deliverable | Specification                                                                                                                                                                                                                                                                 |
|--------| ----------- |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 0a     | License | MIT                                                                                                                                                                                                                                                                           |
| 0b     | Documentation | We will cover new-added features in documentation and usage examples.                                                                                                                                                                                                         |
| 1      | Precise methods definitions | Refine definitions and bahavior of contracts methods (i.e. methods' arguments and returns), depending on namespace, call options and properties of the method, like `payable` & `mutable`. E.g. preamptive querying for transaction calls, controlled by a call options flag. |
| 2      | Methods' names | Format methods' names in the output from original `MethodTrait::method_name` to more user-friendly `methodName` naming scheme, while resolving overlap in formatted names.                                                                                                    |
| 3      | Contract classes extension | Extend generated contract classes with useful properties, normally available on the contract (e.g. address, name, signer, etc.). Rely on usage experience in doing so.                                                                                                        |
| 4      | IDE hints | Prepare generated code to have more informattive IDE hints, based on both JSDoc and output typesystem itself (if needed). Rely on usage experience in doing so.                                                                                                               |
| 5      | NPM Package | Translate package's code to JavaScript upon deployment. Provide informattive CLI, when needed. Make sure to have a cross-platform CLI support.                                                                                                                                |
| 6      | Typechain-compiler | Tool that will be easy-to-use for big projects to compile Rust code and then generate typechain definitions.                                                                                                                                                                  |                                                                                                                                                                                               |

After this grant, we will be maintaining the project to keep up with new emerging ecosystem standards and also listen to issues from community and update the tool to make the process of transformation a nicer experience for the developers and teams.


## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?**

Have a number of approved applications:
- OpenBrush
- Sol2Ink
- Typechain-polkadot (Milestone 1)