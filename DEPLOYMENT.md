# Commercial deployment: WordPress and Zoho

The deployment consists of a customer-owned WordPress website on a live hosting service and components installed directly in the customer's Zoho organization. A managed host, private server or VPS can host WordPress. Zoho widget files are uploaded to and hosted by Zoho CRM; users open them inside CRM. No separate application server is needed to host these widget files.

| Component | Where it runs | How it is installed |
| --- | --- | --- |
| WordPress portal plugin | Customer's live WordPress hosting account | Upload the licensed, approved plugin ZIP through WordPress administration |
| Zoho CRM widget | Zoho CRM, with Zoho internal hosting | Upload the widget ZIP in Setup → Developer Hub → Widgets, select Zoho hosting and set its entry page |
| Schema Setup companion | Zoho CRM administrator workspace | Upload its own ZIP; inspect metadata and explicitly apply supported missing definitions |
| CRM Deluge functions | Customer's Zoho CRM organization | Create the functions with the supplied categories/arguments, then bind the required CRM workflows/buttons |
| Projects / Writer / Sign connections | Customer's Zoho-managed connections | Authorize the required service and scopes in that account |

## WordPress installation on the live host

1. Obtain the licensed release approved for the intended deployment. Confirm its supported WordPress/PHP versions and release status. Public showcase repositories are not WordPress plugin ZIPs.
2. Have a restorable backup of website files and database. Confirm the exact domain, hosting account and WordPress installation before changing it.
3. In that site's WordPress administration, open **Plugins → Add New Plugin → Upload Plugin**. Choose the supplied plugin ZIP, install it, and activate it when the release's migration and dependency requirements are met. A hosting administrator can deploy files through the host's supported management tools if dashboard upload is unavailable.
4. Configure the business identity, portal pages, services, service area and enabled modules. Set the site's HTTPS URL and any callback URLs to its real domain.
5. Store CRM credentials and signing keys only in the protected server-side configuration prescribed by the plugin. Restrict private files/evidence to the release's approved storage outside the public document root. Configure backup retention, outbound HTTPS, maintenance and operational monitoring with the host.

PowerPortals is currently under development and its production release gates are not met. Its development package blocks production initialization. The steps above describe the intended commercial deployment of an approved release; they do not authorize bypassing that guard or installing a development snapshot over a working site.

## Connect the live WordPress installation to Zoho

1. In the intended Zoho organization, identify the integration user, regional service domains, required modules and permitted actions.
2. Configure OAuth through the plugin's supported server-side integration. Register the exact HTTPS callback supplied by that release on the customer's live domain. Authorize only the required scopes and verify the connected organization/user in the integration settings.
3. Review module and field mappings against that account's actual API names. Schema Setup can create supported missing definitions after administrator review; formulas, relationships and unavailable definitions may still need manual work. Mapping discovery is not the same as activating a mapping.
4. Install dependent functions and native CRM workflows/buttons in Zoho. Configure Projects, Writer and Sign connections only where the purchased capability needs them.
5. Where signed CRM-to-WordPress events are enabled, configure the real HTTPS receiver endpoint, key identifier and secret on the appropriate protected sides. Verify signature checks, timestamp/replay handling, delivery errors and access revocation. Do not publish secrets or put them in widget JavaScript.
6. Verify the end-to-end path with controlled test records: website submission → intended CRM record → approved follow-up → permitted portal visibility. Test the reverse path only for the events and changes the release explicitly supports. Uploading a widget alone does not establish WordPress synchronization.

Use the hosting provider's staging environment and a Zoho sandbox for account-specific acceptance before enabling customer traffic. These are hosted release-validation environments, separate from the commercial production destination. Record the release versions, mappings, connection ownership, update procedure and recovery plan before handover.

## Install Zoho widgets directly in Zoho CRM

1. Download the component ZIP and its Schema Setup ZIP from the approved release. Keep their checksums and version record.
2. Sign in to the intended Zoho CRM organization as an authorized administrator. Open **Setup → Developer Hub → Widgets** and create a widget.
3. Select the component's documented type, choose **Zoho** for hosting, and upload its ZIP. Enter the exact index page listed in the component's INSTALL.md, then save.
4. Attach it to the intended record button, related list, dashboard, Web Tab or Settings component. Upload alone does not place the widget in a user's workspace. Record-bound widgets need the correct module and record context.
5. Install Schema Setup as its own administrator widget, inspect the plan, choose access profiles and explicitly apply supported missing definitions. Finish manual definitions and required functions/connections/workflows before enabling dependent actions.
6. Confirm layout access, record permissions, expected reads/writes and operational ownership. Enable the customer-facing workflow only after the release and account acceptance criteria pass.

Private servers may host WordPress and any explicitly required server-side integration service. These Zoho products use Zoho internal hosting; customer installation does not require a terminal, Linux packages or a development web server.

## Official platform references

- [WordPress plugin installation](https://wordpress.org/documentation/article/manage-plugins/)
- [Zoho widget upload and placement](https://www.zoho.com/crm/developer/docs/widgets/usage.html)
