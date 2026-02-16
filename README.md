# ISPConfig 3 Server Manager for FOSSBilling

> ⚠️ **Project Archived – No Longer Maintained**
>
> This repository has been **archived** and is no longer actively maintained.
>
> Development has been discontinued due to the declining usage of ISPConfig 3 and the age of the platform. While the module may continue to function in existing environments, no further updates, fixes, or compatibility improvements are planned.
>
> You are welcome to fork and maintain your own version if you wish to continue development.

---

## Overview

This repository provides an ISPConfig 3 server manager module for FOSSBilling.

The module was rewritten to utilize the ISPConfig 3 RESTful API and was developed and maintained as a community-driven package.

Because this project is archived, it should **not be considered production-supported software**. Use at your own discretion.

---

## Installation (Legacy / Manual)

1. Download the `Ispconfig3.php` file from the source code.
2. Copy the downloaded `Ispconfig3.php` file to `/library/server/manager/Ispconfig3.php`in your FOSSBilling instance.

> ⚠️ Manual installation is required. No automated installer or future compatibility updates will be provided.

---

## Custom Package Values

The following custom package parameters are supported:

- `vat_id` — Default: `NULL`
- `web_php_options` — Default: `no,fast-cgi,cgi,mod,suphp,php-fpm`  
> Note: Availability of these options depends on your ISPConfig 3 configuration.
- `limit_shell_user` — Default: `1`
- `ssh_chroot` — Default: `no,jailkit,ssh-chroot`
- `language` — Default: `en`
- `pm_process_idle_timeout` — Default: `30`
- `pm_max_requests` — Default: `30`
- `mailserver` — Default: `1`

---

## Fine-Tuning Hosting Package Settings

> [!NOTE]  
> If you do not define these custom values in the package, they will default to `-1` (unlimited) unless otherwise specified below.

Additional configurable limits:

- `max_mail_domains`
- `max_mail_aliases`
- `max_mail_alias_domains`
- `max_mail_forwarders`
- `max_mail_catchall`
- `max_mail_filters`
- `max_fetchmail`
- `mail_quota`
- `limit_spam_policy`
- `max_cron_jobs`
- `limit_cron_frequency` — Default: `5` minutes

---

## Disclaimer

This module is provided as-is, without warranty or guarantee of compatibility with newer versions of FOSSBilling or ISPConfig 3.

No further feature development, bug fixes, or security updates are planned.

