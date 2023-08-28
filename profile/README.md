# eduTAP

[:construction: DRAFT :construction:]

eduTAP as "educational tapping", derived from the marketing term "tap to pay" / "tap to open" / "tap to ride" by Apple and Google, describing the act of "tap" a smartphone on a reader device to perform a transaction. 

In educational context a person can tap their smartphone (with specifc passes in the wallet) to:

- identify themself
- pay
- open a door
- lent a book
- take a campus shuttle
- ...

eduTAP tries to fulfill the vision of the [European Student Card](https://erasmus-plus.ec.europa.eu/european-student-card-initiative/card), by establishing a state-of-the-art "common identity document" (ISO/IEC 18013-5 based) for members of education institutions and providing a common way to access on-site services, while respecting holders privacy and other european legal requirements.

## Goals :dart:

Our goals:

The **European digital campus card on the smartphone**:

- for Europe and the world
- decentralized
- secure and state of the art
- compliant (e.g. GDPR, vendor neutral)
- updates easily possible
- accessible
- follow european juridication requirements
- community governed free and open source software 
- favourable adaption possible

We do *not* want: :stop_sign:

- own apps on the smartphone: we use the existing wallets (e.g. Apple Wallet, Google Wallet) or relevant planed wallets (e.g. European Digital Identity Wallet, openWallet Foundation Wallet) and incorporate existing apps where needed (for example Erasmus+ App)
- new protocols or specifications
- providing commercial software
- competition with other projects or providers

## Initiatives :framed_picture:

The big picture of the project.
The project is managed agilely and the initiatives from which we create epics are:


1. eduTAP documentation

   

1. eduTAP-Core (Generic) :avocado:
   
   Necessary software to easily create a "common identity pass" or specific service passes for an issuing institution (normaly a Higher Education Instition (HEI)) and issuing those passes to potential credential holders. 

   - Connect to wallet / pass providers like Google, Apple or Host Card Emulations (HCE) like Legic, NXP or HID with a unified Wallet Communication API (Wallet-API)
   - Provide Callback Applications and event delegation 
   - Provide a generic Pass Issuing Management Portal
   - Provide a generic Pass Issuing Frontend
   - Provide a generic Pass Designer 

1. eduTAP-Libs (Generic) :factory:

   Generic libraries and sample apps, which can be used to implement a specific application to read a pass from the smartphone
    
   - configurable VAS / Smarttap library to read Apple VAS passes, or Google Smarttap passes
   - configurtable ISO/IEC 18013-5 library to read an eduTAP Common ID pass
   - app to check student status
   - checkin to a course 
   - checkin to an exam

1. Central Service Directory :plate_with_cutlery:

   - Provide a management system to announce services (like a library, canteen, lab access) on Higher Education Institutes (HEIs) to a central directory.
   - Provide a search portal to find services and information how to get the digital passes to access these services.
   - Provide a REST API to include the directory entries in the HEI portal.
   - Provide micro search portals for HEIs without resources to integrate in their own portal. Offer simple customization features (style/ logo overrides)

1. Infrastructure and Deployment :bento:

   Since the core applications are planned to run in every HEIs infrastructure we plan to provide detailled instructions how to use eduTAP from a system administration point of view.

   We plan to offer ready to use containers for the reusable parts of the system, ready to run on Docker, Kubernetes (and othe OCI compatible platforms).

1. Mandant Specific Applications (MasA) :arrow-right: eduTAP@institution :hamburger:

   Every Heigher Education Instituition (HEI) has different ways to store data, offer services, use hardware etc.
   We plan to provide examples for more generic services and generic programming libraries to not reinvent the wheel for every HEI.


## State :footprints:

Project planning and prototype.

## Read More :open_book:

Read the documentation of the projects predecessor [ECC-Pilot](https://ecc-pilot.github.io/documentation/)

In future read our own documentation (t.b.d.)
