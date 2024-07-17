# Overview

## What is the Nasir Platform?

The Nasir Platform is an online service tailored for KNTU students, offering a range of services that complement or enhance existing university offerings.

Operated as an open-source initiative, the platform is governed by a decentralized autonomous organization (DAO) comprised of students. It encourages contributions in development, advertising, bug fixing, problem-solving, and funding from individuals of all backgrounds.

The Nasir Platform also serves as a hub for students interested in computer science, providing opportunities to actively engage, refine skills, and develop tools used in daily academic life.

## High-Level Design

The Nasir Platform operates with two primary layers:

1. **Layer 1 (L1)**: This encompasses critical systems like authentication, crypto systems, the DAO, and AI frameworks. Users typically do not interact directly with L1 systems, which form the foundational infrastructure supporting the platform's applications.
    
2. **Layer 2 (L2)**: This layer includes user-facing applications such as advanced data gathering systems, community forums, educational wikis, and transactional tools like Snapp Eshteraki and book exchanges.
    

### Layer 1

L1 systems are crucial to the Nasir Platform's operation. These components collaborate to form the foundation of the platform, enabling the functionality of the different L2 applications.

#### Authentication System

The platform employs four authentication tiers:

1. **Biganeh**: Limited access to select L2 programs, requiring only an email address or Ethereum/TON wallet for registration.
2. **Shahrvand**: Full access granted to current KNTU students, staff, or faculty members through university-issued credentials.
3. **Dev**: Members of CSSA Clubs with access to specific codebases authorized by their respective clubs. Devs can hold either Biganeh or Shahrvand status.
4. **Hakem**: DAO members of Nasir Coin with full access privileges across all L2 applications, governed by DAO guidelines.

|           | Authentication Method | L2 App Access          | Privacy Level |
| --------- | --------------------- | ---------------------- | ------------- |
| Biganeh   | Email or wallet       | Restricted             | High          |
| Shahrvand | Student ID or Uni ID  | Full                   | Low           |
| Dev       | Club verification     | Specific club projects | Low           |
| Hakem     | DAO membership        | Full                   | Low           |

#### Nasir Coin (Crypto System)

Nasir Coin serves as an internal currency within the platform, facilitating transactions across most L2 apps. It is not limited to KNTU students, enabling global transactions akin to Bitcoin or gold. It can also be viewed as store of value.

Let's explore the practical uses of Nasir Coin within the Nasir Platform:

- Honeypot projects can be incentivized with Nasir Coin.
- Extra projects in university subjects can be rewarded with Nasir Coin.
- Open-source developers will receive Nasir Coin as a reward.
- Club registration fees, courses, and events can be paid with Nasir Coin.
- Books and notes can be exchanged using Nasir Coin.
- Food codes can be exchanged using Nasir Coin.
- Loan mechanisms can be facilitated through external funding projects using Nasir Coin.

Full implementation details is in [Nasir Coin whitepaper](link) .
#### Internal Wallet (Crypto System)

The internal wallet simplifies Nasir Coin transactions and ensures user security by managing private keys securely. Integration with MetaMask allows users additional control over their Nasir Coins outside the platform's internal system.

#### DAO

The Decentralized Autonomous Organization (DAO) governs Nasir Platform development process and ensures funds are used to benefit the platform and its student community. DAO operations are executed transparently using blockchain technology, specifically Ethereum.

#### AI Systems

AI/ML models within the Nasir Platform support functions like content moderation in forums, community engagement in NPC forums and preventing duplication in Senfi Yar, with future expansions planned for additional L2 apps.

#### Account Management

A dedicated module manages user accounts and integrates seamlessly with the platform's authentication and crypto systems.

### Layer 2

L2 modules are designed to directly address student needs and facilitate interactions on the platform.

#### SenfiYar

###### Description

In the Senfi Yar program, users can share their Senfi-related issues in a manner similar to Reddit. Other users can view these posts, upvote or downvote them, and leave comments. Users have the option to remain completely anonymous or participate using their registered identity. Unlike typical forums or platforms like Reddit, official Senfi members are required to respond to issues with evidence, track the progress of specific problems, and report back on Senfi Yar or their channels.
This program enhances transparency regarding university issues, improves communication between students and Senfi, strengthens the university community, and ultimately leads to a better understanding and resolution of problems.
###### Access Level

Viewing is open to all, but interaction requires Shahrvand status.

#### NPC

###### Description

The Nasir Programming Contest (NPC) is a system that tracks and stores participants' points in contests. It functions similarly to Quera, allowing for the creation and management of contests or managing links to existing Quera contests. Winners are rewarded with Nasir Coin through this module.
###### Access Level

Viewing is open to all, while interaction requires Biganeh status.

#### Nasir Wiki/Forum

###### Description

A student-driven forum and wiki covering KNTU-related topics, providing a repository of information on professors, subjects, administrative details and many other unwritten rules and knowledge crafted by elder student to guide inexperienced students.

###### Access Level

Viewing is open to all, with interaction privileges reserved for Shahrvand members.

#### Currency Exchange

###### Description

Allows users to exchange Nasir Coins for other cryptocurrencies like Tether and Ether, enhancing transaction flexibility.

###### Access Level

Available to Biganeh users for transactions.

#### Book & Note Exchange

###### Description

Facilitates the buying, selling, donating, and sharing of academic materials among students.

###### Access Level

Interaction requires Biganeh status.

#### Food Code Exchange

###### Description

Enables students to exchange meal vouchers, enhancing convenience and reducing food wastage.

###### Access Level

Selling requires Shahrvand status, while buying is accessible to Biganeh users.

#### Data Gathering System (DGS)

###### Description

Supports statistical data collection and surveys, benefiting academic research and student projects.

###### Access Level

Accessible exclusively to Shahrvand members.

#### Autonomous Nasir Newspaper

###### Description

A decentralized platform for student-generated articles and news, fostering free expression and community engagement.

###### Access Level

Open to Biganeh users for publication and interaction.

#### Snapp Share

###### Description

Facilitates ride-sharing among students, improving transportation options.

###### Access Level

Exclusive to Shahrvand users.

# How to Build and Who?

### Development Process

The Nasir Platform is developed collaboratively by CSSA programming clubs specializing in AI, Web Development, Blockchain, and Network & Security. Each club handles specific modules assigned to them, integrating their work with other clubs' contributions.

For detailed development guidelines of projects in Clubs, documentation available [here](link).

### Contributors

Development efforts are led by club members who are passionate about learning and building practical solutions. Participation is open to all, including those outside KNTU who wish to join the clubs and contribute.

* club members are given "Dev" status
 
# Where to Use?

Users primarily access the platform via web browsers, with plans for cross-platform compatibility. Telegram integration further enhances accessibility through mini-apps, bots, and APIs, particularly beneficial for features like the Nasir Newspaper.

# Future

### Vision

The Nasir Platform is designed to evolve dynamically, adapting to emerging needs while upholding principles of transparency, free speech, and user privacy. Governed by its student community via DAO, it should remain resilient against external influence.

### Inspiration

Inspired by Ethereum's decentralized ethos and open-source principles, the Nasir Platform the Nasir Platform emphasizes decentralization, adaptability, transparency, and collaborative development, driving its creation.
# Investment

The platform sustains development through investments in Nasir Coin and advertising, ensuring continuous improvement and expansion.

# Challenges and Considerations

- **Execution Challenges**: Implementing such a complex platform requires robust technical expertise, especially in blockchain, AI/ML, and web development. Ensuring consistency and reliability across all modules will be critical.
    
- **Community Adoption**: While the document outlines open participation, ensuring active involvement and engagement from a diverse student body may require effective community management and incentivization strategies.
    
- **Governance and Regulation**: Balancing decentralized governance with compliance and university regulations could pose challenges, especially regarding financial transactions and data privacy.
    
- **Sustainability**: Continuous funding and income generation through Nasir Coin investments and advertising are crucial for long-term sustainability. Ensuring a stable economic model and avoiding misuse of resources will be essential.