# W3F Open Grant Proposal

* **Project Name:** OpenBrush
* **Team Name:** [SuperColony](https://github.com/Supercolony-net)
* **Payment Address:** ERC 20 ADDRESS:
0x112C9eDB60D16f9Cf501721b03B9D0F275682213

## Project Overview :page_facing_up:

### Overview

OpenBrush is open source library for secure smart-contract development on ink! as
[OpenZeppelin](https://github.com/OpenZeppelin/openzeppelin-contracts) on Solidity.

But in addition to implementing standard contracts,
it will also provide additional functionality to simplify
the smart-contract development process and documentation with examples.

As the last stage of the library, the team will contribute to ink! and `contract-pallet`.

### Project Details

The open brush should be the starting point for smart contract developers from Ethereum. 
It will contain the same folder structure and documentation that describes the differences 
between ink! and Solidity, how developers should change their mindset, how to design their project, 
how to deploy contract and test them, etc.

The library will provide the default implementation of standard contracts which 
can be customized by developers. Also, the library will provide additional 
features which are not available in ink!(and our team will try to integrate them into ink! later) 
but which can be useful for development.

Our team aims to improve the smart-contract development experience,
and wants to improve ink! to popularize it.

### Ecosystem Fit

* Where and how does your project fit into the ecosystem?
  
The project fits in any substrate-based blockchain because 
  it can have `contract-pallet` which provides ink! support.
* Who is your target audience (parachain/dapp/wallet/UI developers, designers, your own user base, some dapp's userbase, yourself)?

Our target audience is smart contract developers.

* What need(s) does your project meet?

Our project is starting point for smart contract developers from Ethereum and it aims to improve smart contract development on ink!.

* Are there any other projects similar to yours in the Substrate / Polkadot / Kusama ecosystem?
  
We know only about one project [metis](https://github.com/patractlabs/metis).

* If so, how is your project different?

Our project wants not only to provide the default implementation of contracts.
It aims:
- Provide the default implementation of popular contracts.
- Simplify reuse/customization of implementations from the library.
- Defines standards for ink! (We've already created [PSP](https://github.com/w3f/PSPs/pull/22) for fungible tokens and we plan to create more)
- Be an entry point for smart-contract developers from Ethereum(provide accord documentation).
- Contribute to ink! to improve the smart-contract development experience(add new features, fix bugs, etc).
- Contribute to `contract-pallet` to add support of upgradable contracts.

## Team :busts_in_silhouette:

### Team members

**Markian Ivanichok** (Founder)  
**Dmitry Kryshtal** (Marketing and BD)  
**Green Baneling** (Blockchain Core Developer)  
**Sven Seven** (Fullstack Developer)  
**Varg Vikernes** (Junior Blockchain Engineer)  
**Lera Laricheva** (Intern Creative Designer)  
**Ian Arden** (Advisor)  
**Hartej Sawney** (Advisor)  


### Contact

* **Contact Name:** Dmitry Kryshtal
* **Contact Email:** dmitry.kryshtal@supercolony.net
* **Website:** [supercolony.net](supercolony.net)

### Legal Structure

* **Registered Address:** Dubai Silicon Oasis, DDP, Building A2, Dubai, UAE. 
* **Registered Legal Entity:** Mempool Ventures FZCO, operating unde Supercolony brand

### Team's experience

Please describe the team's relevant experience. If your project involves development work, we would appreciate it if you singled out a few interesting projects or contributions made by team members in the past. For research-related grants, references to past publications and projects in a related domain are helpful.

**Markian Ivanichok**
CEO of Supercolony
Blockchain enterpreneur, Lead Software Engineer
Started my engineering carrer back when I was 15th. Since then developed and got lots of experience in engineerig and leadership. Got entrepreneur experience by founding a couple of startups in soft. Inspired, co-founded and invested in Sector F, on of the top consulting companies in Ukraine that help enterpreneers to move faster. 
Since the beginning of this year co-founded and led Supercolony, a Polkadot venture studio that is dedicated to building and creating of Polkadot’s ecosystem.


**Dmitry Kryshtal**  
8 years experienced T-Shaped marketer with a deeper understanding of analytics, creativity and strategy. Opinion leader in the cryptocurrency environment since 2017. Co-owner of the creative agency Citadel. Host of his own program on biggest crypto-related YouTube channel in CIS – S3XYBTC.




**Green Baneling**  
Blockchain Core Developer  
Primary programming languages are: C++, Go, Rust  

Finished the faculty of applied mathematic(Master of degree). Participated in programming competitions during education. Working as a programmer for around 6 years.  

First-year was a freelancer, creating an application for IOS(Swift), creating modules for the desktop application on C++. After that 2 years in the company which creating software for TV devices(C++/ Haxe). After that 3 years on different blockchain projects(C++/Go/Rust/Solidity/Js).




Varg Vikernes
Junior Blockchain Engineer
Was working in Big Data prior to blockchain, now switched to developing on Polkadot and have zero regrets




**Sven Seven**  
Fullstack Developer  
Software engineer with prod experience since 2015. Master degree Information Security. Was working in finance, e-commerce, networking domains as full-stack dev. Programming languages are JS, Java, Python, Rust, C++ . Blockchain dev since 2021.




**Lera Laricheva**  
Creative Designer  
"In 2019 I started to get involved in the IT area. At first I tried myself as a developer, and eventually I went away from that to design. At first I tried myself in design, then when I saw the result and understood that I liked it, I found courses and got a diploma. Then I tried freelancing, like many other beginners, but came to the conclusion that the work in the company is much better, and that is where a person can get a tremendous experience, always evolving, because you have to keep up with the tasks, and most importantly to understand them and try to implement them correctly. At the same time I’m studying the third year in Karazin, specialty marketing."



If anyone on your team has applied for a grant at the Web3 Foundation previously, please list the name of the project and legal entity here.

### Team Code Repos

* https://github.com/Supercolony-net


Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

* https://github.com/VargSupercolony
* https://github.com/sventime
* https://github.com/xgreenx
* https://github.com/PierreOssun

### Team LinkedIn Profiles (if available)

* https://www.linkedin.com/in/mivanichok/
* https://www.linkedin.com/in/ian-arden/
* https://www.linkedin.com/in/hartej/
* https://www.linkedin.com/in/dmitry-kryshtal/
* https://www.linkedin.com/in/valeria-laricheva/
* https://www.linkedin.com/in/valeria-laricheva/

## Development Status :open_book:

[The project](https://github.com/Supercolony-net/openbrush-contracts) already in progress.
TODO

If you've already started implementing your project or it is part of a larger repository, please provide a link and a description of the code here. In any case, please provide some documentation on the research and other work you have conducted before applying. This could be:

* links to improvement proposals or [RFPs](https://github.com/w3f/General-Grants-Program/tree/master/rfp-proposal) (requests for proposal),
* academic publications relevant to the problem,
* links to your research diary, blog posts, articles, forum discussions or open GitHub issues,
* references to conversations you might have had related to this project with anyone from the Web3 Foundation,
* previous interface iterations, such as mock-ups and wireframes.

## Development Roadmap :nut_and_bolt:

This section should break the development roadmap down into milestones and deliverables. Since these will be part of the agreement, it helps to describe _the functionality we should expect in as much detail as possible_, plus how we can verify and test that functionality. Whenever milestones are delivered, we refer to this document to ensure that everything has been delivered as expected.

Below we provide an **example roadmap**. In the descriptions, it should be clear how your project is related to Substrate, Kusama or Polkadot. We _recommend_ that the scope of the work can fit within a three-month period and that teams structure their roadmap as 1 milestone ≈ 1 month.

For each milestone,

* make sure to include a specification of your software. _Treat it as a contract_; the level of detail must be enough to later verify that the software meets the specification.
To assist you in defining it, we have created a document with examples for some grant categories [here](../src/grant_guidelines_per_category.md).
* include the amount of funding requested _per milestone_.
* include documentation (tutorials, API specifications, architecture diagrams, whatever is appropriate) in each milestone. This ensures that the code can be widely used by the community.
* provide a test suite, comprising unit and integration tests, along with a guide on how to set up and run them.
* commit to providing Dockerfiles for the delivery of your project.
* indicate milestone duration as well as number of full-time employees working on each milestone.
* **Deliverables 0a-0d are mandatory for all milestones**, and deliverable 0e at least for the last one. If you do not intend to deliver one of these, please state a reason in its specification (e.g. Milestone X is research oriented and as such there is no code to test).

> :zap: If any of your deliverables is based on somebody else's work, make sure you work and publish _under the terms of the license_ of the respective project and that you **highlight this fact in your milestone documentation** and in the source code if applicable! **Teams that submit others' work without attributing it will be immediately terminated.**

### Overview

* **Total Estimated Duration:** Duration of the whole project (e.g. 2 months)
* **Full-Time Equivalent (FTE):**  Average number of full-time employees working on the project throughout its duration (see [Wikipedia](https://en.wikipedia.org/wiki/Full-time_equivalent), e.g. 2 FTE)
* **Total Costs:** Amount of payment in USD for the whole project. The total amount of funding _needs to be below $30k for initial grants_ and $100k for follow-up grants. (e.g. 12,000 USD). This and the costs for each milestone need to be in USD; if the grant is paid out in Bitcoin, the amount will be calculated according to the exchange rate at the time of payment.

### Milestone 1 Example — Implement Substrate Modules

* **Estimated duration:** 1 month
* **FTE:**  2
* **Costs:** 8,000 USD

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

* **Estimated Duration:** 1 month
* **FTE:**  1
* **Costs:** 4,000 USD

...


## Future Plans

We're going to make strong impact on community, making ink! simple and convenient for developers.

* how you intend to use, enhance, promote and support your project in the short term, and
* the team's long-term plans and intentions in relation to it.


## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** Web3 Foundation Website / Medium / Twitter / Element / Announcement by another team / personal recommendation / etc.

Here you can also add any additional information that you think is relevant to this application but isn't part of it already, such as:

* Work you have already done.
* Wheter there are any other teams who have already contributed (financially) to the project.
* Previous grants you may have applied for.
