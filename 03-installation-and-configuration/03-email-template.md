# Email Template (puqownCloud notification disk limit)

### ownCloud module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/whmcs-module-owncloud.php) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-ownCloud/) | [FAQ](https://faq.puqcloud.com/)

## Creating the email template

Navigate to **System Settings** → **Email Templates** → **Create New Email Template**

---

## Template configuration

| Parameter | Value |
|-----------|-------|
| **Email Type** | Product/service |
| **Unique Name** | puqownCloud Notification disk limit |

---

## Email subject

```
Disk space usage {$disk_used_percentage} % - {$username}
```

---

## Email body

```
Dear {$client_name},

This letter informs you that the disk space usage limit is coming to an end.

Product/Service: {$service_product_name}
Due Date: {$service_next_due_date}

Username: {$username}

Disk limit: {$disk_limit_bytes*$unit_coefficient} {$unit}
Disk used: {$disk_used_unit} {$unit} ({$disk_used_percentage} %)
Disk free: {$disk_free_unit} {$unit} ({$disk_free_percentage} %)


{$signature}
```

---

## Available template variables

The following custom variables are passed to the email template by the module:

| Variable | Description | Example |
|----------|-------------|---------|
| `{$username}` | ownCloud username | john-42 |
| `{$disk_limit_bytes}` | Total disk quota in bytes | 10737418240 |
| `{$unit_coefficient}` | Coefficient for unit conversion | 1073741824 |
| `{$unit}` | Disk space unit | GB |
| `{$disk_used_unit}` | Used disk space in configured unit | 8.5 |
| `{$disk_free_unit}` | Free disk space in configured unit | 1.5 |
| `{$disk_used_percentage}` | Used space as percentage | 85 |
| `{$disk_free_percentage}` | Free space as percentage | 15 |

In addition, all standard WHMCS product/service merge fields are available (e.g. `{$client_name}`, `{$service_product_name}`, `{$service_next_due_date}`, `{$signature}`).

> **Note:** Notifications are sent automatically during the WHMCS daily cron execution when disk usage reaches the threshold configured in the product settings ("Notify at %").

---

## Screenshots

![Email template creation](../img/07-email-template-1.png)
*07-email-template-1.png*

![Email template configuration](../img/08-email-template-2.png)
*08-email-template-2.png*
