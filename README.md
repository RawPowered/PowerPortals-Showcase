<p align="center">
  <img src="assets/powerportals-logo.svg" alt="PowerPortals" width="440">
</p>

<h1 align="center">PowerPortals</h1>

<p align="center"><strong>Business portals that fit the way your company works.</strong><br>
Bring customer, sales, and project workflows together through a branded WordPress experience.</p>

<p align="center">
  <a href="#what-powerportals-is">Product overview</a> ·
  <a href="#portal-suite">Portal suite</a> ·
  <a href="#getting-started">Setup guide</a> ·
  <a href="#release-status">Release status</a>
</p>

---

## What PowerPortals is

PowerPortals is a modular portal platform for WordPress. It is being prepared to help organizations give customers and internal teams a clear place to complete common business workflows, while adapting the experience to each company’s brand and CRM configuration.

The product is in pre-release validation. This public repository is the **product overview and documentation home**; it intentionally does not contain PowerPortals plugin source code or installable packages.

## The portal suite

PowerPortals is being organized as a suite of focused portal experiences. Exact module availability depends on the release and license selected.

| Portal or module | What it is designed to support |
| --- | --- |
| **Customer Portal** | A branded customer-facing place to access relevant service and project information. |
| **Sales and Onboarding Portal** | Guided intake and onboarding workflows that collect information needed to start a customer relationship. |
| **Project Portal** | Project-facing views and actions for coordinating work with customers and teams. |
| **BOM add-on** | Bill of materials workflows, offered as an optional module. |
| **Commissions add-on** | Commission-related workflows, offered as an optional module. |

The goal is to configure only the modules a company needs, then expand the suite as its workflow grows.

## CRM setup and field mapping

The first integration focus is **Zoho CRM**. A setup guide is being shaped to walk administrators through connection setup, organization and user verification, required modules, and the fields each enabled portal needs.

PowerPortals is being prepared to adapt to CRM installations that already exist. The setup experience will identify required data, help map a company’s CRM fields to portal fields, and make missing prerequisites clear. Zoho is the initial target; broader CRM API support and assisted field mapping must be validated for each provider before they are described as generally available.

For early testing, use a dedicated CRM sandbox and a separate WordPress test site. Keep production credentials and customer data out of test environments.

## Getting started

PowerPortals is not yet published as a public plugin download. When a licensed release is available, the intended onboarding flow is:

1. Install the supplied PowerPortals package on a supported WordPress site.
2. Open the setup guide and enter the company name, brand assets, and portal preferences.
3. Choose the portal modules included in the license.
4. Connect Zoho CRM in a sandbox first, then verify the organization and authorized user.
5. Review the required CRM modules and map the fields used by each enabled workflow.
6. Run the setup checks, review access settings, and publish the portal pages when validation passes.

The exact requirements, supported versions, and distribution instructions will be documented with the first release.

## Product principles

- **Brand adaptable:** company identity and portal presentation should be configurable rather than tied to one customer’s brand.
- **Workflow aware:** setup should explain what each enabled portal requires and surface missing CRM prerequisites.
- **Modular:** optional capabilities can be licensed and enabled independently where supported.
- **Security minded:** integrations should use scoped credentials, protect secrets, and be tested in a sandbox before production use.
- **Transparent:** compatibility, module status, and setup requirements should be clear before installation.

## Release status

PowerPortals is in active productization and release-gate testing. The descriptions here communicate product direction; they are not a claim that every module, CRM provider, or distribution workflow is generally available today. Availability and commercial terms will be announced with a verified release.

## Screenshots and demonstrations

Verified product screenshots and short demonstrations will be added here as release-ready assets become available. Images will be reviewed to remove customer information, credentials, and other private data before publication.

## Security

Please do not post credentials, tokens, customer records, or private vulnerability details in public issues. A dedicated private security reporting method will be published before general availability. Until then, use this repository for public product and documentation feedback only.

## Repository scope

This repository is for public product information, setup documentation, and release announcements. It does not grant a license to PowerPortals software, trademarks, or other product materials. Plugin source code and licensed installation packages are distributed separately under the terms provided with a commercial release.

---

<p align="center"><strong>PowerPortals</strong><br>One portal suite. Configured for your business.</p>
