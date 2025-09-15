# 2 Description

{% hint style="success" %}
Set the context of the Building Block for the reader. The description should not assume that the reader has any experience of the GovStack system other than that found on the GovStack website.

If there are assumptions or context for this building block that may be needed for the reader, it can be provided in this section.
{% endhint %}

## 2.1 Premise

The CMS Building Block is a comprehensive model for the standardization of government websites, through the use of content management systems (CMS). By extension, it also covers the websites of all public institutions, including central agencies, local and regional administration, embassies, other public authorities, and educational institutions.

The GovStack CMS building block prescribes CMSs as the basis for websites offering citizens access to government information and services. For a definition of a CMS, see 3 Terminology.

The CMSs must be able to utilize and integrate with other GovStack Building Blocks. The model therefore uses three overarching criteria to ensure compatibility with the [Building Blocks concept](https://govstack.gitbook.io/specification/building-blocks/about-building-blocks) and the requirements of a government use case. CMSs should be:

* Built for interoperability and easy integration.
* Respecting open standards, preferably using open source.
* Designed for scale, flexibility, and upgradability.

## 2.2 Coverage

The specification includes a comprehensive conceptualization of the following organizational and operational fields, including related technical and methodological capacity-building and training programs:&#x20;

* Planning
* Governance
* Development
* Deployment
* Hosting
* Security
* Maintenance
* Content management

## 2.3 Flexibility

The specification can be adapted to the ecosystem of each country, accounting for differences in:

* Stakeholder perspectives&#x20;
* Local technical readiness
* Availability of technical capacity for all relevant roles (see implementation strategy for a list of relevant roles)
* Regulatory framework
* Technical methodologies and culture of technical peer collaboration
* Available funding sources
* Development cooperation actors (if relevant for the country context)

## The Role of CMSs in Government and Public Administration <a href="#the-role-of-cmss-in-government-and-public-administration" id="the-role-of-cmss-in-government-and-public-administration"></a>

### Information and services reflecting the country <a href="#information-and-services-reflecting-the-country" id="information-and-services-reflecting-the-country"></a>

Maintaining a modern and effective web presence is a fundamental necessity for all governments and public institutions. It is achieved through a well-planned, well-executed, and well-maintained information delivery based on one or more online content management systems.

Government websites are a window to the country, reflecting its identity, giving access to the most important and up-to-date information, as well as to key public services, for the citizens, companies, investors, and tourists. Without a well-designed, performant website, which allows users to accomplish their tasks, trust in government diminishes.&#x20;

Thus, government web portals have two major functions:

* Delivery of up-to-date information in a well-structured and accessible manner.
* Provide an entry point to electronic public services (e-services)

### Standardizing for consistent governance, quality, and efficiency <a href="#standardizing-for-consistent-governance-quality-and-efficiency" id="standardizing-for-consistent-governance-quality-and-efficiency"></a>

In order to achieve these goals efficiently, the governmental web portals need to be secure, performant, scalable, attractive, accessible, and user-friendly. Government websites must present a cohesive content structure that allows quick information retrieval and effective navigation.&#x20;

The users should have a consistent service experience across all institutions and their online properties, following the same informational flow and reflecting a common visual identity. Behind the scenes, applying unified governance principles across hosting, development, and maintenance processes is crucial to minimize costs, resource consumption, security risks, and reduce dependency on external service providers. This centralized approach ensures efficiency and security across diverse government operations.

These considerations are not only true for the central government organization. They should also apply to regional and local institutional entities. These websites also provide information and services to citizens, businesses, and other interested stakeholders.

### Establishing a digitally sovereign platform <a href="#establishing-a-digitally-sovereign-platform" id="establishing-a-digitally-sovereign-platform"></a>

There are significant benefits in evolving a single national governance model covering the following institutional categories:

* Central government, including ministries and top-most institutions (e.g., presidency, parliament, prime minister’s office, etc.)
* National government agencies
* Regional and local governments (e.g., provinces, districts, municipalities, and other administrative units)
* Embassies and other diplomatic missions of the country

Digital sovereignty is always important when establishing this platform, so the government can ensure that it maintains ownership of data, retains control over digital assets, and avoids vendor lock-in.

### Creating opportunities for the national economy <a href="#creating-opportunities-for-the-national-economy" id="creating-opportunities-for-the-national-economy"></a>

The life cycle of the websites created through this building block should provide opportunities for job creation and sustainable business opportunities for local companies. All services required for the development, maintenance, hosting, monitoring, upgrading, extending, and integrating the websites could generate new business and create employment opportunities for local talent.

## Standardizing the life cycle of government websites <a href="#standardizing-the-life-cycle-of-government-websites" id="standardizing-the-life-cycle-of-government-websites"></a>

The critical mission of government and public institution websites is to keep citizens and other stakeholders informed and to provide entry points to e-services. This makes it imperative to establish good governance models that can ensure the continuity, resilience, accessibility, and coherence of the websites and related supporting processes.&#x20;

#### Central standardization goals <a href="#central-standardization-goals" id="central-standardization-goals"></a>

The standardization should aim to ensure:

* Coherent and consistent presentation of information to the stakeholders. Information should be structured predictably, where the website’s content taxonomy and availability of services can be identified with ease.
* Consistent identity, styling, and user experience design that allows easy navigation in the informational structure and rapid identification of the next steps to achieve end-user goals.
* Consistent ways for website editors to manage content. Editors from all institutions should be able to follow public documentation for content editing and use the same approaches to complete the same tasks.
* Effective and efficient technical development and evolutive maintenance at low cost and with low risk will allow central governance of the technical processes. They can be executed by a compact, dependable, and predictable development capacity with predictable training goals that cover updates, upgrades, development of additional features, integration of additional components, etc.
* Coherent planning, implementation, and management of the hosting infrastructure, following the same rules for continuous integration (CI), continuous deployment (CD), and monitoring, to ensure proper security, performance, accessibility and availability.

### Minimum general requirements <a href="#minimum-general-requirements" id="minimum-general-requirements"></a>

The standardization concept requires that a government website meets high requirements for:

* Security
* Scalability
* Accessibility and inclusiveness
* Extendability
* Integrability&#x20;

### Lifecycle components requiring standardization <a href="#lifecycle-components-requiring-standardization" id="lifecycle-components-requiring-standardization"></a>

The lifecycle components that require standardization are:

* Development
* Routine maintenance
* Feature enhancements
* Upgrades, updates, and repairs
* Contribution to upstream libraries/code/documentation
* Integration
* Deployment and hosting
* Performance monitoring
* Cybersecurity auditing and security monitoring
* Accessibility auditing, reporting and monitoring
* Disaster recovery
* Technical support
* Technical project management
* Content editing
* Content migration
* Training and onboarding for content editors

## Strategic governance of government website implementation and maintenance <a href="#strategic-governance-of-government-website-implementation-and-maintenance" id="strategic-governance-of-government-website-implementation-and-maintenance"></a>

### Common negative effects of a decentralized approach <a href="#common-negative-effects-of-a-decentralized-approach" id="common-negative-effects-of-a-decentralized-approach"></a>

Traditionally, the responsibility to implement institutional websites has been delegated to each individual institution or its immediate administrative superior.&#x20;

&#x20;

Deeply rooted institutional autonomy and lack of centralized standard guidelines and regulations have often led to the perpetuation of an ad-hoc approach where each public institution is responsible for the entire life cycle of its own website, encompassing conceptual development, content structure, technical architecture, implementation (or contracting of development services), maintenance, hosting, upgrades, extensions, integrations, security, performance, accessibility, replacement/disposal and data migration.

### Benefits of a centralized standardization approach <a href="#benefits-of-a-centralized-standardization-approach" id="benefits-of-a-centralized-standardization-approach"></a>

A centralized approach to governance is central to a successful strategic standardization of government websites. It will ensure coherent management and decision-making, as well as reduce the cost and management overheads associated with widely distributed management approaches.

Centralized and standardized governance models have already been established for the websites of central governments. In some cases, it has also been extended to other categories of public institutions as well.

Relevant examples of government website standardization are those of the United Kingdom, Peru, Germany, and Rwanda (this list may not be exhaustive or complete.)

### Management with clearly defined accountability <a href="#management-with-clearly-defined-accountability" id="management-with-clearly-defined-accountability"></a>

Centralized and standardized governance requires that the management of the entire life cycle of the websites is assigned to and taken on by a single institution or a group of institutions under a single clearly defined accountability agreement.

Such a governance structure must contain at least the following:

* Benchmarking and identification of the optimal CMS technology, following this specification.
* Planning the development and the rollout of new websites and the migration of information assets.
* Ensure the application of relevant rules and guidelines. For example, graphic identity, accessibility, domain naming, hosting, and monitoring.
* Train and support the technical capacity required to define, specify, supervise, and evaluate the technical implementation tasks.
* Plan for major evolutive maintenance operations, such as major technological upgrades.
* Ensure technical support participating institutions.
* Train and support the content editors of participating institutions..
* Identify, competitively procure, and assign the technical capacity that can provide development and maintenance activities when needed.
