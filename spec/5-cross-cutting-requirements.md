# 5 Cross-Cutting Requirements

{% hint style="success" %}
The Cross-cutting requirements described in this section are an extension of the cross-cutting requirements defined in the architecture blueprint and nonfunctional requirements document. This section will describe any additional cross-cutting requirements that apply to this building block, or any requirements that are defined in the non-functional requirements document that are NOT applicable to this Building Block.

Cross-cutting requirements will use the same language (REQUIRED, RECOMMENDED or OPTIONAL) as specified in the architecture document.

Note: this section will contain 3 parts. The first is a list of Requirements, followed by any exceptions to the cross-cutting requirements for this building block (this section may be skipped if not needed). The third part is a list of relevant standards to this domain that should be used for any Building Block implementation.
{% endhint %}

This section describes essential requirements that apply to the software and processes involved in this building block.&#x20;

Wherever applicable, the term CMS also includes third-party components (i.e., extensions, plugins, modules) necessary to achieve the functionality required by the building block.

## Security (REQUIRED) <a href="#security-required" id="security-required"></a>

The framework must ensure a high level of security, including, but not limited to:&#x20;

* Multi-Factor Authentication (MFA)
* Industry-standard encryption algorithms
* Including files stored outside the web root and granular access rights for assets, files, and folders
* Triggerable password resets from the backend
* Granular access control for the administrators and site editors

and other secure practices which should be followed by default

The CMS must have at least:

* Maintenance by a dedicated team
* Security announcements with a subscription option (e.g. through email)
* A dedicated security team
* Documented process for managing security bugs
* No conflicting software licenses

CMS’s should also have:

* Accessibility teams and public feedback systems
* A defined sustainability practice&#x20;

Non-core code (modules, extensions, plugins) should be curated to minimize the risk of introducing security vulnerabilities.

## Multi-tenant capabilities (REQUIRED) <a href="#multi-tenant-capabilities-required" id="multi-tenant-capabilities-required"></a>

The CMS must allow multiple websites and web domains to run on one instance of the CMS, using a single or shared codebase that can be used to deploy common resources to multiple instances. This will allow upgrades, patches, and functional additions or changes to be propagated on all websites that run on the same instance.

Sharing of content and backend user accounts should also be possible between individual websites.

## Multilanguage and content translation (REQUIRED) <a href="#multilanguage-and-content-translation-required" id="multilanguage-and-content-translation-required"></a>

The CMS must allow straightforward setup and management of languages and translation of content and UI using an API.

## Availability and scalability (REQUIRED) <a href="#availability-and-scalability-required" id="availability-and-scalability-required"></a>

The run-time stability and reliability of the functional components in the CMS must be documented through independent quality review and evidence of use within the government sector.

Operational stability with data sets and traffic volumes appropriate for the government use case should also be ascertained. The CMS must adapt seamlessly to growing traffic and increasing amounts of content, including media/photos. It must have an efficient approach to managing large databases of media assets. It should support the generation of optimized assets on rendered web pages to ensure page loading performance.

## Configurability (REQUIRED) <a href="#configurability-required" id="configurability-required"></a>

The CMS must be highly configurable without the use of procedural programming or changes to core files.

The configuration should be deployable as configuration files or code.

Frontend output must allow compliance with any existing government design style guides.

## Predictable upgradability (REQUIRED) <a href="#predictable-upgradability-required" id="predictable-upgradability-required"></a>

The CMS must be updatable with a predictable and minimal risk of breaking functionality on patch releases.

The CMS must provide documentation on breaking changes and deprecations. Breaking changes should be introduced predictably in major releases, unless the breaking change is introduced to mitigate a security issue that cannot be mitigated through other measures.

The CMS should have a predictable upgrade roadmap to ensure that the website is kept up to date as the technologies evolve, that it remains secure, and that its underlying technology is continuously maintained.

Each version of the CMS should have an expected release lifecycle, including the length of official support (the period of time during which bug fixes and security patches are provided after initial release). This will enable the length of the lifecycle to be matched with the expected lifecycle of the government websites.

## Extensibility (REQUIRED) <a href="#extensibility-required" id="extensibility-required"></a>

The functionality of the CMS must be extensible through third-party components (i.e., extensions, plugins, modules) without changing the code of the CMS itself.

It must be possible for the implementation team of this building block to use their self-developed components with the CMS.

## Open source license (RECOMMENDED) <a href="#open-source-license-recommended" id="open-source-license-recommended"></a>

The CMS platform and its source code should be available under an open source [license approved by the Open Source Initiative (OSI)](https://opensource.org/licenses).

## A broad community of contributors (RECOMMENDED) <a href="#a-broad-community-of-contributors-recommended" id="a-broad-community-of-contributors-recommended"></a>

The CMS should have a wide international community of technical developers that maintain expertise and contribute to the development of the platform and additional components.

The community should be governed by a published code of conduct and be conducive to the sharing of knowledge and experience.

## Deployability (REQUIRED) <a href="#deployability-required" id="deployability-required"></a>

The CMS must support the completion of effective automated deployment to remote servers and cloud solutions without accessing the CMS’s graphical user interface.

The technical interventions on the websites should follow a proper continuous integration and continuous deployment (CI/CD) process to ensure that the production environments remain stable and available continuously and that replicable on-deploy upgrade functionality can be implemented, for example, in development and live environments&#x20;

## Search Engine Optimization (SEO) and machine readability  (REQUIRED) <a href="#search-engine-optimization-seo-and-machine-readability-required" id="search-engine-optimization-seo-and-machine-readability-required"></a>

The CMS must allow granular management of SEO properties on a per-page basis in order to ensure good performance for the pages in external search engines, such as Google.

The CMS must include support for fundamental SEO functionality, such as meta description fields and site map generation.&#x20;

Machine readability, in particular through large language models (LLMs), is an evolving area and an important part of this requirement.

## Accessibility  (REQUIRED) <a href="#accessibility-required" id="accessibility-required"></a>

The CMS’s frontend output must be able to natively support the technical requirements of web standards, such as the Web Content Accessibility Guidelines (WCAG), as well as any applicable national requirements. This will ensure that the content is accessible to all website visitors, including those with visual or motor impairments. It should support WCAG 2.2 or newer, at least Level AA.

## Workflow and Versioning (RECOMMENDED) <a href="#workflow-and-versioning-recommended" id="workflow-and-versioning-recommended"></a>

The CMS should support data publication workflows that allow content to be prepared without instantaneous publication. It should also have the possibility for publication processes involving multiple levels of review and approval before publishing.

The CMS should also include a detailed history function that allows reverting of published content and establishes an audit trail for all content.

## Differentiated backend user permissions (REQUIRED) <a href="#differentiated-backend-user-permissions-required" id="differentiated-backend-user-permissions-required"></a>

The CMS must support differentiated group-based user permissions that allow numerous editors to access and manage only the content that lies within their purview. This is important both for security and governance.

Permissions should at least cover these areas:

* Differentiation between view only and changing content.
* Assignable access to websites, sections of websites, and individual pages.
* Possibility to limit editing to particular content types.
* Access to document and media storage structures within a more extensive digital asset repository.
* Differentiation between view only and changing digital assets like documents and media.

## Data import and export (REQUIRED) <a href="#data-import-and-export-required" id="data-import-and-export-required"></a>

The CMS must support bulk data import and export through a well-documented API or standardized and open file formats.

## Data decoupling (RECOMMENDED) <a href="#data-decoupling-recommended" id="data-decoupling-recommended"></a>

The CMS should employ a high degree of decoupling (i.e., separation) between content data and view/design information.
