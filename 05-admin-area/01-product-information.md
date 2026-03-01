# Product Information

### ownCloud module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/whmcs-module-owncloud.php) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-ownCloud/) | [FAQ](https://faq.puqcloud.com/)

## Admin area product information

The administrator can view detailed service information in the WHMCS admin panel on the product/service page. The module adds a custom panel in the **Module Data** section with the following information:

### License verification status

Displays the current license status with a colored indicator:
- **Green** — license is valid and active
- **Red** — license is invalid, expired, or missing

### API connection status

Shows the result of a real-time connection test to the ownCloud server, confirming that the API credentials are working correctly.

### User information

| Field | Description |
|-------|-------------|
| **Username** | The ownCloud username assigned to this service |
| **Enabled** | Whether the user account is currently enabled or disabled |
| **Group** | The ownCloud group(s) the user belongs to |
| **Email** | The email address associated with the ownCloud account |

### Disk usage

- **Visual progress bar** — a colored bar showing the proportion of used vs. free disk space
- **Detailed table** with:
  - Disk limit (total allocated quota)
  - Disk used (current usage)
  - Disk free (remaining space)
  - Disk used percentage
  - Disk free percentage

### Available management actions

The standard WHMCS module command buttons are available:
- **Create** — provision a new ownCloud account
- **Suspend** — disable the ownCloud user
- **Unsuspend** — re-enable the ownCloud user
- **Terminate** — permanently delete the ownCloud user
- **Change Password** — reset the user's password
- **Change Package** — update disk quota and group assignment (used during upgrades/downgrades)

---

## Screenshot

![Admin area product information](../img/14-product-information.png)
*14-product-information.png*
