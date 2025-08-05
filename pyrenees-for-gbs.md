## Product Requirements Document: Pyrenees for GBS
#### Version: 2.0 (Final)
#### Date: August 5, 202
#### Author: Gemini Pro Web Design / Martin Ferrero-Thompson

#### 1. Overview & Vision
This document outlines the requirements for a single-page promotional and fundraising website for a charitable cycle ride across the Pyrenees. The rider, a person who has lived through Guillain-Barré Syndrome, is undertaking this challenge to raise awareness and funds for three national GBS support agencies: GBS-CIDP Foundation International (UK), Asociación Española de GBS-PFS y MFS (Spain), and Association Française GBS-PFS et MFS (France).

The website's primary goals are:

    1.  Inspire & Connect: To tell a powerful personal story of resilience and hope.

    2. Educate: To provide clear, accessible information about Guillain-Barré Syndrome.

    3. Drive Donations: To create a clear and trustworthy path for visitors to donate directly to their regional GBS agency.

The overall feel is modern, hopeful, and professional. The design uses powerful imagery, clean typography, and a user-friendly layout to build trust and encourage engagement.

#### 2. Core User Experience: The Portal
The website uses a "portal-first" approach to deliver a tailored experience to each user.

* Automatic Language Detection:

    * On first load, the site will automatically detect the user's browser language.

    * If the language is Spanish (es) or French (fr), the site will load the corresponding version directly, bypassing the portal.

    * For all other languages (including English), the site will default to the English version.

* Portal Landing Page:

    * This page serves as a manual selection screen and a clear entry point.

    * Layout: A full-screen hero image with a central panel.

    * Content:

        * The full title: "Pyrenees for Guillain-Barré Syndrome".

        * A clear statement of purpose: "A charity ride to raise awareness and support."

        * Three prominent, clickable flag buttons (UK, Spain, France) for users to select their preferred regional experience. The Spanish button is subtly enlarged to signify the main partnership.

* Seamless Transition: Once a language is selected (either automatically or manually), the portal fades out and the main website content fades in.

#### 3. Technical Stack & Implementation
* Structure: A single, semantic HTML file.

* Styling: Tailwind CSS for a utility-first, responsive design.

* JavaScript: Vanilla JavaScript for all dynamic functionality.

#### 4. Global Elements
#### 4.1. Fixed Navigation Bar
The navbar remains fixed at the top of the viewport, becoming semi-transparent with a blur effect on scroll.

* Logo:

    * Content: Text-based logo: "GBS".

    * Functionality: Acts as a "home" button. Clicking it fades out the main site and fades the portal back in, allowing users to re-select their region.

* Navigation Links:

    * Smooth-scroll links to the corresponding sections on the page.

    * Links: The Story, The Ride, About GBS, The Charity, Sponsors, Updates.

    * Language: All link text is displayed in the user's selected language.

    * Responsiveness: Font sizes and spacing adjust on smaller screens to ensure the text remains on a single line.

* Theme Selector:

    * An icon that cycles through Light, Dark, and System modes. The user's preference is saved in local storage.

#### 4.2. Floating Social Panel
A vertical bar fixed to the left side of the viewport with icons linking to relevant social media profiles.

#### 5. Page Sections
#### 5.1. Hero Section
* Layout: Full-screen with a high-quality background image of the Pyrenees.

* Content: A powerful headline and sub-headline (in the selected language) and a primary "Support the Ride" button that scrolls to the Charity section.

#### 5.2. The Story Section
* A two-column layout featuring a photo of the rider and their personal narrative.

#### 5.3. About GBS Section
* Layout: A clean, centered content block with a stylish accordion interface.

* Accordion Style:

    * Each item has clear visual separation.

    * A "plus" icon smoothly animates to a "minus" when an item is opened.

    * The active item has a subtle background highlight for clarity.

* Content: Three expandable sections explaining GBS, the recovery path, and the role of support agencies.

#### 5.4. The Ride Section
A visually engaging section with a map of the route and key statistics (Distance, Elevation, Days).

#### 5.5. The Charity Section
* Functionality: This section displays only one charity card, corresponding to the language/region selected by the user.

* Content: The title and descriptive text are tailored to the specific charity (e.g., "Support Our UK Partner"). The card contains the charity's logo, a brief description, and a direct link to their official donation page.

#### 5.6. Sponsors Section
* A grid of current sponsor logos and a clear call-to-action block for potential new sponsors to make contact via a mailto: link.

#### 5.7. Updates / Blog Section
* A grid of cards for posting updates. Each card includes an image, date, title, and snippet.

#### 5.8. Footer
* Contains a mailto: link for general inquiries, logos of all three partner charities, and website credits.
