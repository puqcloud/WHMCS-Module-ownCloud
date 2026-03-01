# Add server (ownCloud server)

### ownCloud module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/whmcs-module-owncloud.php) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-ownCloud/) | [FAQ](https://faq.puqcloud.com/)

## Adding an ownCloud server to WHMCS

Navigate to **System Settings** → **Servers** → **Add New Server**

---

### Step 1: General settings

Enter the correct **Name** and **Hostname** for your ownCloud server.

- **Name** — a descriptive name for the server (e.g. "ownCloud Production")
- **Hostname** — the domain name or IP address of your ownCloud installation (e.g. `cloud.example.com`)

If your ownCloud uses a non-standard port, enter it in the **Port** field. Check the **Secure** checkbox if your server uses HTTPS (recommended).

![Add server - general settings](../img/04-add-server-1.png)
*04-add-server-1.png*

---

### Step 2: Module settings

1. In the Server Details section, select the **PUQ ownCloud** module from the dropdown
2. Enter valid credentials for the ownCloud web interface:
   - **Username** — ownCloud administrator username
   - **Password** — ownCloud administrator password
3. Click **Test connection** to verify the connection is working correctly

The test connection verifies that the module can reach the ownCloud OCS API (`/ocs/v1.php/cloud/users/`) and authenticate with the provided credentials.

![Add server - module settings](../img/05-add-server-2.png)
*05-add-server-2.png*

> **Important:** The ownCloud user must have **administrator privileges** to manage users via the API. The module uses the ownCloud OCS API v1 with HTTP Basic Authentication to create, modify, suspend, and delete user accounts.
