# eduTAP

[DRAFT]

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

- own apps on the smartphone: we use the existing wallet and incorporate existing apps where needed (for example Erasmus+ App)
- new protocols or specifications
- providing commercial software
- competition with other projects or providers

## Initiatives :framed_picture:

The big picture of the project.
The project is managed agilely and the initiatives from which we create epics are:

1. Core (Generic) :avocado:
   
   - Connect to pass providers like Google, Apple or Host Card Emulations (HCI) like Legic, NXP or HID with a unified Wallet Communication API (Wallet-API).
   - Povide Callback Applications and event delegation. 
   - Provide a Pass Issuing Management Portal.
   - Provide a Pass Issuing Frontend

3. Mandant Specific Applications (MasA) :hamburger:

   Every Heigher Education Instituition (HEI) has different ways to store data, offer services, use hardware etc.
   We plan to provide examples for more generic services and generic programming libraries to not reinvent the wheel for every HEI.


2. Central Service Directory :plate_with_cutlery:

   - Provide a management system to announce services (like a library, canteen, lab access) on Higher Education Institutes (HEIs) to a central directory.
   - Provide a search portal to find services and information how to get the digital passes to access these services.
   - Provide a REST API to include the directory entries in the HEI portal.
   - Provide micro search portals for HEIs without resources to integrate in their own portal. Offer simple customization features (style/ logo overrides)


4. Infrastructure and Deployment :bento:

   Since the core applications are planned to run in every HEIs infrastructure we plan to provide detailled instructions how to use eduTAP from a system administration point of view.

   We plan to offer ready to use containers for the reusable parts of the system, ready to run on Kubernetes or Docker Swarm (and othe OCI compatible platforms).

## State :footprints:

Project planning and prototype.

## Read More :open_book:

Read the documentation of the projects predecessor [ECC-Pilot](https://ecc-pilot.github.io/documentation/)

In future read our own documentation (t.b.d.)




