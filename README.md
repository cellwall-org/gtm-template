# CellWall Google Tag Manager Template

Official Google Tag Manager template for installing CellWall Cookie Consent and synchronizing visitor choices with Google Consent Mode v2.

## Features

- Loads the CellWall browser agent using a CellWall project ID.
- Sets restrictive consent defaults before other GTM tags run.
- Maps CellWall Analytics, Marketing, and Functional choices to Google Consent Mode v2.
- Updates GTM consent state when a visitor changes their CookieWall preferences.

## Installation

Until the template is accepted into the GTM Community Template Gallery, download `template.tpl` from this repository and import it in **Templates → Tag Templates → New → Import**.

Create a tag using **CellWall Cookie Consent**, enter the project ID from the [CellWall dashboard](https://platform.cellwall.io/), and trigger it on **Consent Initialization - All Pages**.

See the [installation guide](https://cellwall.io/en/resources/blog/gtm-installation) for complete setup and validation steps.

## Consent mapping

| CellWall category | Google consent types |
| --- | --- |
| Marketing | `ad_storage`, `ad_user_data`, `ad_personalization` |
| Analytics | `analytics_storage` |
| Functional | `functionality_storage`, `personalization_storage` |
| Strictly Necessary | `security_storage` |

## Review status

The Gallery submission is awaiting re-review after addressing [issue #1](https://github.com/cellwall-org/gtm-template/issues/1) with the GTM Consent APIs.

## License

This project is licensed under the [Apache License 2.0](LICENSE).
