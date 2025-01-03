# eduTAP

eduTAP as "educational tapping", derived from the marketing term "tap to pay", "tap to open", and "tap to ride" by Apple and Google, describing the act of "tap" a smartphone on a reader device to perform a transaction.

In an educational context, a person can tap their smartphone (with specific passes in the wallet) to:

- identify themself,
- claim a discount,
- pay,
- open a door,
- lend a book,
- take a campus shuttle,
- ...

eduTAP plans to fulfill the interoperability vision of the [European Student Card](https://erasmus-plus.ec.europa.eu/european-student-card-initiative/card), by establishing a state-of-the-art "common identity document - eduID" (["ISO/IEC 18013-5:2021 Personal identification — ISO-compliant driving licence — Part 5: Mobile driving licence (mDL) application"](https://www.iso.org/standard/69084.html) based) and dedicated services passes for members of education institutions and providing a common way to access on-site services, while respecting holder's privacy and other European legal requirements.

eduTAP also plans by its name and design to line up with other services provided by [Géant](https://geant.org/) within the [Géant Trust and Identity Services](https://geant.org/services/trust-and-identity-services/):

- [eduGAIN](https://edugain.org/)
- [eduroam](https://eduroam.org/)
- [eduTEAMS](https://eduteams.org/)
- *[InAcademia](https://inacademia.org/)*

Disclaimer: eduTAP is currently a project by the "European University Alliance" [EUGLOH (European University Alliance for Global Health)](https://eugloh.eu/) and not an official Géant Service or Product. It is in the concept and pilot phase (multiple prototypes), proving to the responsible DG EAC that an inter-university campus can provide interoperable services for its own and incoming HEI members.

## Goals :dart:

Our goals:

The **European digital campus card on the smartphone**:

- for Europe and the world,
- decentralized,
secure and state-of-the-art,
- compliant (e.g. GDPR, vendor-neutral),
- updates are easily possible,
- accessible,
- follow European jurisdiction requirements,
- community-governed free and open-source software,
- favourable adaption possible.

We do *not* want: :stop_sign:

- own apps on the smartphone: We use the existing wallets (e.g. Apple Wallet, Google Wallet) or relevant planned wallets (e.g. "European Digital Identity Wallet", "openWallet Foundation Wallet") and incorporate existing apps where needed (for example Erasmus+ App),
- new protocols or specifications,
- providing commercial software,
- competition with other projects or providers.

It facilitates the "Law of Gall":

> A complex system that works is invariably found to have evolved from a simple system that worked.
> A complex system designed from scratch never works and cannot be patched up to make it work.
> You have to start over with a working simple system.
>
> <cite>John Gall - Systemantics: How Systems Really Work and How They Fail</cite>

and builds on top of fantastic existing concepts, technologies, and software. We do not try to create a complex system from scratch, but just connecting existing technology, like building a bridge.

## Initiatives :framed_picture:

The big picture of the project.
The project is managed agilely and the initiatives from which we create epics are:


1. eduTAP-Core (Generic) :atom:

   The necessary software to easily create a "common identity pass" or specific service passes for an issuing institution (normally a Higher Education Institution (HEI)) and issue those passes to potential credential holders.

   - Connect to wallet / pass providers like Google, Apple, or Host Card Emulations (HCE) like Legic, NXP, or HID with a unified Wallet Communication API (Wallet-API),
   - provide Callback Applications (event delegation),
   - provide a generic "Pass Issuing Management Portal", including a generic "Pass Designer",
   - provide a generic "Pass Issuing Frontend" (web and kiosk modes).

1. Central Service Directory :plate_with_cutlery:

   - Provide a management system to announce services (like a library, canteen, and lab access) on Higher Education Institutes (HEIs) to a central directory.
   - Provide a search portal to find services and information on how to get the digital passes to access these services.
   - Provide a REST API to include the directory entries in the HEI portal.
   - Provide micro search portals for HEIs without resources to integrate with their portal. Offer simple customization features (style/ logo overrides)

1. Mandant Specific Applications (MasA) :arrow_right: eduTAP@institution :hamburger:

   Every Higher Education Institution (HEI) has different ways to store data, offer services, use hardware, etc.
   We plan to provide examples for more generic services and generic programming libraries to not reinvent the wheel for every HEI.

   Generic support libraries for the MaSA, and sample apps, which can be used to implement a specific application to read a pass from the smartphone

   - configurable VAS / Smarttap library to read Apple VAS passes, or Google Smarttap passes,
   - configurable ISO/IEC 18013-5 library to read an eduTAP Common ID pass,
   - app to check student status,
   - check-in to a course,
   - check-in to an exam.

1. Infrastructure and Deployment :bento:

   Since elements of the core applications are planned to run in every HEI's infrastructure we plan to provide detailed instructions on how to use eduTAP from a system administration point of view.

   We plan to offer ready-to-use containers for the reusable parts of the system, ready to run on Docker, Kubernetes (and other OCI-compatible platforms).

1. [eduTAP documentation](https://docs.edutap.eu/) :books:

   Documentation about eduTAP, the components, and technologies.


## State :footprints:

- project planning
- implement wallet APIs
- further planning 

## Read More :open_book:

Read our [documentation](https://docs.edutap.eu/) or go to our [eduTAP website](https://edutap.eu)
