# 6 \_previously listed as Data structures&#x20;

## Database — structured data storage and decoupling <a href="#database-structured-data-storage-and-decoupling" id="database-structured-data-storage-and-decoupling"></a>

The CMS should employ a high degree of decoupling (i.e., separation) between content data and end-user presentation. It is advantageous for governments to store data both highly structured and decoupled. It is important to differentiate the use of structured and relational data and true decoupling of design and data information.&#x20;

Data decoupling will allow higher performance on operations involving extraction of more atomic data entities because they employ database queries, rather than searches within larger data blobs. Such extraction tasks could for example “all images on a page” or “extract all headings for a table of contents.”

Data decoupling will also allow more effortless reuse of data on other platforms, implementing the possibility of increased use of single redundancy in the data space.

## Media files and documents — flexible locations and asset management <a href="#media-files-and-documents-flexible-locations-and-asset-management" id="media-files-and-documents-flexible-locations-and-asset-management"></a>

The CMS should support flexible referencing of files that allows for file storage in multiple locations, not necessarily on the hosting server. This enables efficient file storage, interaction with document management systems, and increased access security for vital files.

The CMS should support file taxonomy and metadata management, either within the core or with a deeply integrated digital asset management (DAM) system.

## Configuration — versioned and differentiated by site and environment  <a href="#configuration-versioned-and-differentiated-by-site-and-environment" id="configuration-versioned-and-differentiated-by-site-and-environment"></a>

The CMS should support configuration within versioned configuration files in a way that supports domain-dependent configuration. Configuration should be able to be stored outside the database and should enable the use of different configurations for different sites and deployment environments.

## Code — deployable and versioned, separate from data <a href="#code-deployable-and-versioned-separate-from-data" id="code-deployable-and-versioned-separate-from-data"></a>

All source code must be deployable separately to data in media files, documents, and databases. The CMS must thus support the implementation of replicable on-deploy upgrade functionality for differing data sets, for example, in development and live environments.

The CMS should support the use of a dependency manager, such as Composer for PHP, Maven/Gradle for Java, or NPM for JavaScript.
