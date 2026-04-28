<p align="center">
  <img src="https://www.seven.io/wp-content/uploads/Logo.svg" width="250" alt="seven logo" />
</p>

<h1 align="center">seven SMS for Vtiger CRM</h1>

<p align="center">
  Plug seven into the <a href="https://www.vtiger.com/">Vtiger CRM</a> SMS Notifier as a provider for outbound SMS.
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-teal.svg" alt="MIT License" /></a>
  <img src="https://img.shields.io/badge/Vtiger-7.x-blue" alt="Vtiger 7.x" />
  <img src="https://img.shields.io/badge/PHP-7.x%2B-purple" alt="PHP 7.x+" />
</p>

---

## Features

- **SMS Notifier Provider** - Drop-in provider for the Vtiger SMS Notifier module
- **Bulk Send from List Views** - Select records in *Contacts*, *Organizations* etc. and SMS them in one action
- **Custom Sender ID** - Optionally override the displayed sender per provider configuration

## Prerequisites

- [Vtiger CRM](https://www.vtiger.com/) 7.x with the SMS Notifier module enabled
- A [seven account](https://www.seven.io/) with API key ([How to get your API key](https://help.seven.io/en/developer/where-do-i-find-my-api-key))

## Installation

### Via terminal

```bash
wget https://raw.githubusercontent.com/seven-io/vtiger/master/Seven.php \
  -P /path/to/vtigercrm/modules/SMSNotifier/providers
```

### Via FTP

1. Download the [`Seven.php`](https://github.com/seven-io/vtiger/blob/master/Seven.php) provider file.
2. Upload it to `Vtiger/modules/SMSNotifier/providers/` on your server.

## Configuration

1. In the Vtiger admin, click the **SMS Notifier** tab.
2. Click the wrench icon and select **Server configuration**.
3. Click **New configuration** and fill in:

| Field | Description |
|-------|-------------|
| Provider | Select `seven` |
| Active | Tick to activate |
| API Key | Your seven API key |
| From | Optional sender ID |

4. Save the form and enable the *seven* provider for sending SMS.

## Usage

### Send SMS from a list view

1. Open a module (e.g. *Contacts*, *Organizations*).
2. Tick the records you want to message.
3. Click **Actions > Send SMS**.
4. Type the message and click **Send**.

## Support

Need help? Feel free to [contact us](https://www.seven.io/en/company/contact/) or [open an issue](https://github.com/seven-io/vtiger/issues).

## License

[MIT](LICENSE)
