<p align="center">
  <img src="assets/powerportals-logo.svg" alt="PowerPortals" width="380">
</p>

<h1 align="center">PowerPortals</h1>

<p align="center"><strong>One branded experience. A clearer path from first inquiry to active work.</strong><br>
Customer intake, sales handoff, and project communication—built around the way your business works.</p>

<p align="center">
  <a href="#the-powerportals-experience">The experience</a> ·
  <a href="#features-in-development">Features</a> ·
  <a href="#designed-to-fit-your-business">Built around your business</a> ·
  <a href="#availability">Availability</a>
</p>

---

> **Pre-release:** PowerPortals is in active development and validation. PHP 8.3 is the current development target and has passed automated checks and an isolated WordPress test. The features below describe the product direction; they are not a public software release or a promise that every capability is ready for production.

## The PowerPortals experience

PowerPortals is a modular portal platform for WordPress. It is being developed to give prospective customers, customers, and internal teams a consistent place to start and manage service workflows—under the business’s own brand.

The aim is to make the handoff feel connected: a prospective customer explains what they need, the team receives a useful lead record, and customers who choose to create an account can return to follow their work or start another request.

## Features in development

### Guided lead intake and service quotes

Replace a generic contact form with a guided, step-by-step service request. Prospective customers can describe their goals, choose the services that apply, share timing and budget context, and provide photos of the space or property. Service categories and accepted states are intended to be configurable for each installation.

### Property details for location-based work

For property-related requests, the intake is designed to collect an address, let the customer verify or adjust its map pin, and look up available parcel details such as folio number and legal description. Florida parcel lookup is being developed as an add-on. Public records and map references are supporting context for review; they do not establish ownership or replace an official county record.

### Zoho lead handoff

Zoho CRM is the first integration target. The planned handoff connects submitted intake details to a mapped lead workflow, with setup guidance for the organization, authorized user, required modules, and fields. CRM connectivity and live lead handling still require validation before a general release.

### Optional customer account

After submitting a request, a lead is intended to be able to create a customer account immediately, with the account marked **Pending Approval** while the team reviews the project. The portal is optional: a project can be declined or not proceed while the account remains available for future requests. New project requests are designed to sit alongside an archived prior request.

### A modular portal suite

The broader suite is planned to include focused experiences for customer access, sales and onboarding, and project coordination, with optional BOM and commissions add-ons. Module availability will depend on the release and license.

## Designed to fit your business

- **Your brand:** configure the portal presentation for the organization using it.
- **Your services:** enable the service categories that apply to that business and installation.
- **Your service area:** set a default state and, when needed, restrict accepted states.
- **Your CRM setup:** map portal fields to the existing Zoho configuration and make missing setup requirements visible.
- **Your workflow:** enable only the modules included in the release and needed by the team.

PowerPortals is being designed as a brand-adaptable product. The public overview does not include customer-specific configuration, production credentials, or installable plugin source.

## Intended setup flow

1. Install a licensed PowerPortals package on a supported WordPress site.
2. Configure the organization’s branding, enabled services, and accepted states.
3. Connect a Zoho sandbox, verify the organization and authorized user, and map the fields used by enabled workflows.
4. Review setup and access checks, then publish the portal pages when the release requirements are met.

The final supported-version matrix, setup guide, distribution instructions, and commercial terms will be published with a verified release.

## Availability

PowerPortals is not currently available as a public plugin download. The guided lead-intake and service-quote form, Zoho lead sync, Florida parcel lookup, and optional customer intake portal remain under private development and validation. No public package or general-availability date is being announced yet.

This repository is the public product overview and documentation home. It does not contain plugin source code or installable packages and does not grant a license to PowerPortals software, trademarks, or product materials.

## Security and testing

Integrations are being developed for scoped credentials and sandbox-first validation. Use a dedicated CRM sandbox and a separate WordPress test site for early testing; keep production credentials and customer data out of test environments. Before general availability, each enabled module must be validated against its documented access rules and supported workflow.

Do not post credentials, tokens, customer records, or vulnerability details in public issues. Use the repository’s **Security** tab to report a vulnerability privately.

---

<p align="center"><strong>PowerPortals</strong><br>One portal suite. Configured for your business.</p>
