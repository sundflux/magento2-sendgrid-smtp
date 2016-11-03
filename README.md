# SendGrid SMTP Plugin for Magento2.1
Configure Magento to use SendGrid's SMTP server to send all transactional emails.

*Note:* You need a valid SendGrid account.

Fork of yukoff/magento2-sendgrid-smtp

Initial changes:
- Update composer.json for 2.1
- Fix typos in this readme
- .. other fixes coming if needed.

## 1. Install SendGrid SMTP Plugin
### Using Composer
```
composer require sundflux/magento2-sendgrid-smtp
```

### Using Source Code
```
composer config repositories.sundflux-sendgridsmtp git git@github.com:sundflux/magento2-sendgrid-smtp.git
composer require sundflux/magento2-sendgrid-smtp
```

### Manual Installation
Install SendGrid SMTP plugin for Magento2
 * Download the extension
 * Unzip the file
 * Create a folder {MAGENTO_ROOT}/app/code/SendGrid/SendGridSmtp
 * Copy the content from the unzipped folder

## 2. Enable SendGrid SMTP Plugin
```
php -f bin/magento module:enable --clear-static-content SendGrid_SendGridSmtp
php -f bin/magento setup:upgrade
```

## 3. Config SendGrid SMTP Plugin
Log into your Magento2 backend, then goto `Store -> System -> SendGrid SMTP` and enter your email credentials, SendGrid category (if used) etc.
