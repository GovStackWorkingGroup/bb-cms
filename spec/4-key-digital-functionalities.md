# 4 Key Digital Functionalities

{% hint style="success" %}
The Key Digital Functionalities (KDFs) describe the core (required) functions that this building block must be able to perform. These functionalities should be described as business processes as opposed to technical specifications or API definitions.

The KDFs provides an overview of functionality that should be provided by the Building Block. These KDFs should be organized by area of functionality and should be numbered so that they can be referenced in other sections.

Note, any assumptions or context that are needed for this Building Block should be provided in Section 2 (Description).
{% endhint %}

The Building Block will be accessible through the web browser, through all suitable devices such as desktops, laptops, mobile phones, tablets, and public touchscreen displays.

## Primary user categories <a href="#primary-user-categories" id="primary-user-categories"></a>

The functionalities are divided into two primary categories, depending on the role of the user that is interacting with the CMS:

* **Backend/back-office** functionality is available to website administrators and content editors.
* **Frontend** functionality is available to website visitors (citizens, etc.).

## Terms used for functionalities <a href="#terms-used-for-functionalities" id="terms-used-for-functionalities"></a>

To define functionalities, the following terms will be used:

* **Content block:** A modular section of content within a webpage that is structured as a standalone unit, consisting of text, links, images, videos, or buttons, designed for easy customization, rearrangement, or reuse
* **Grid of content blocks:** A structural element that arranges content blocks within a grid layout. It organizes the content blocks into rows and columns with consistent responsiveness and visual balance when viewed on devices with differing screen sizes.
* **Media:** Any type of content that can be displayed, played, or interacted with on a website. Types of media files include images (JPG, PNG, GIF, SVG, WEBP), PDF files, videos (MP4, embedded YouTube/Vimeo), audio (MP3, WAV, podcasts).
* **Slider:** A component that displays multiple pieces of content, such as images, texts, or videos, as a dynamically changing sequence of image and text slides displayed in the same location, often with a sliding effect transitioning each slide. Users can navigate through the slides manually (by swiping or clicking arrows or dots) or automatically. A slider is also known as a _carousel_.
* **Banner:** A prominent visual element used for branding, promotions, or important messages. It includes text, images, buttons, or animations meant to capture the user’s attention.
* **Accordion:** A user interface component that organizes content into collapsible sections. Each section expands when clicked or tapped, revealing hidden content, and typically collapses when another section is opened.
* **Tabs:** A user interface component and navigational element that organizes content into multiple sections, allowing users to switch between them without leaving the page. An analogy to tabbed dividers in a filing cabinet, each tab represents a different section of content, and only one section is visible at a time.
* **Time-ordered content (News and Events, blog posts):** Information published online, typically covering current events, updates, opinions of current relevance or announcements, presented in article format. A news article commonly consists of title, subtitle, author’s name, date and time of publication (or update), summary, body content (main article), images, videos, categories, tags, and social sharing options. News articles may feature user comments.
* **Backend user:** An individual who has been granted access to the Backend, commonly responsible for creating, editing, and organizing the website’s content and other administrative tasks. The user’s specific capabilities are defined by and tailored to their assigned role and responsibilities.

## Backend functionality requirements <a href="#backend-functionality-requirements" id="backend-functionality-requirements"></a>

This section lists functionalities that are minimum requirements for the CMS backend.

A backend user, depending on its specific allocated rights or roles, must be able to:

* Upload, manage and use files for content creation.
* Create and manage navigational structures and menu items.
* Create and manage content pages.
* Create and manage content blocks of at least the following types or combinations thereof:&#x20;
  * Text
  * Media
  * Image slider
  * Content block slider
  * Banner
  * Table
  * Accordion
  * Tabs
  * File download
  * Time-ordered content (News, Events, Announcements, Blog posts etc)
  * Forms
* Create and manage grids of content blocks.
* Create and manage SEO-relevant settings for each page and content element.
* Create and manage properties that affect accessibility&#x20;
* Create and edit hyperlinks to internal or external web pages.
* Create and manage publishing workflows, including content approval.
* Create and manage content for multiple languages through a visual user interface, enabling comprehensive multi-lingual support.
* Localize and translate pages and content blocks in all available content languages.
* Create new and manage existing websites using a standardized UX
* Copy/cut and paste individual pages or content blocks.
* Copy/cut and paste content structures, such as groups of pages and content blocks.
* Reuse existing content across one or multiple websites while keeping a single editable source (no redundancy).
* Export and import content structures using an open file format or API.
* Create and manage backend users, manage user roles, and set granular permissions.
* Restrict backend user access to specific websites, website sections, or individual pages.

### Frontend functionality requirements <a href="#frontend-functionality-requirements" id="frontend-functionality-requirements"></a>

This section lists functionalities that are minimum requirements for the CMS frontend.

All visitors to the website (frontend users)  must be able to:

* Navigate the content structure using the menu and links.
* Switch between content languages.
* List and read current and historical news articles published on the website.
* Search the website content using keyword search.

The Frontend functionality should be accessible to all users, including those with disabilities.&#x20;

## General functionality requirements <a href="#general-functionality-requirements" id="general-functionality-requirements"></a>

The following functionality requirements affect both backend and frontend user experience.

### Link management system <a href="#link-management-system" id="link-management-system"></a>

The CMS should facilitate the creation of both internal and external hyperlinks. The internal linking mechanism must ensure:

* **Portability and flexibility:** Pages can be moved and renamed without breaking links to them. This also includes maintaining link integrity within the CMS instance when it is replicated and deployed across different environments (e.g., development, staging, and production).
* **Maintenance and consistency:** Editors must be able to update site structure or reassign domains without being required to manually adjust every internal hyperlink.
* **Scalability in Multisite or Multilingual context:** Internal hyperlinks must automatically adapt to the current site and language context.

### File management layer <a href="#file-management-layer" id="file-management-layer"></a>

The CMS must provide a unified and consistent interface for managing files, regardless of their underlying storage location or system. The file management layer must ensure the following:

* **Uniformity:** A single user interface and a single API, whether files are stored locally, on remote servers, or in cloud-based storage
* **Portability:** Ease of migration and scaling of websites across different environments without changing the file management logic. “Environments” in this context refer to development, testing, staging, and production servers, any of these environments being powered by Linux or Windows operating systems. The same applies to the ability to migrate and scale websites to or between local systems and cloud platforms.
* **Flexibility and extensibility:** Allow integration with multiple storage systems and file services, local or remote.
