# Changelog

### ownCloud module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/whmcs-module-owncloud.php) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-ownCloud/) | [Community](https://community.puqcloud.com/)

---

## v4.1.0 (30-09-2026)

- **Isolated Cron Synchronization & Disk Monitoring.** Scheduled disk statistics and usage calculations are now individually protected for each ownCloud service with dedicated error logging. Temporary server unreachability or API timeouts will never abort the daily WHMCS cron job.
- **Strict PHP 8.2+ Compatibility & Type Hardening.** Fully typed property assignments across usage history and quota limits, preventing unexpected type errors on PHP 8.1, 8.2, and 8.3 environments.
- **Zero-Touch Settings Auto-Migration.** Existing ownCloud products automatically upgrade their configuration options into modern unified settings (`configoption24`) directly in the database without manual updates.
- **Enhanced WHMCS 9 Select2 UX & Hook Resilience.** Sidebar menu hooks and admin alerts are guarded by error boundaries, and dynamic settings injection has been upgraded for seamless compatibility with Select2 in WHMCS 9.
- **Clean Module Logging.** Excluded repetitive local database license verification checks (`License_Verification (db)`) from the WHMCS Module Log, logging exclusively online verification transactions to keep diagnostic logs clean.

---

## v4.0.0 (02-09-2026)

- Full compatibility with WHMCS 8.x and WHMCS 9+
- Universal **ionCube Loader v15** support for seamless encoding compatibility
- Modernized administrative product settings interface with dynamic injection and enhanced stability
- Improved client area responsiveness and user session management
- Performance optimizations and enhanced error recovery during automated provisioning tasks

---

## v3.1 (01-03-2026)

- Added null coalescing checks for all array and superglobal accesses to prevent "Undefined array key" warnings
- Added null-safe operators for object property access where object can be null
- Fixed type safety for typed class properties (preventing `TypeError` on null assignment)
- Added boundary checks for empty database query results

---

## v3.0 (21-01-2026)

- Support for WHMCS 9+
- Redesigned product module settings
- Updated client area interface design

> **Note:** Product reconfiguration is required after update.

---

## v2.1 (31-07-2025)

- Fixed bug with uninitialized statistics data variables causing critical errors on statistics page (PHP 8.x)

---

## v2.0 (23-09-2024)

- Module coded with ionCube v15
- Supported PHP versions: 7.4, 8.1, 8.2
- Compatible with WHMCS 8.11.0+

---

## v1.3.1 (13-08-2024)

- Fixed password display bug when "Show password" set to "no"

---

## v1.3 (06-06-2024)

- Mobile-optimized client area
- Added copy buttons for login and password credentials

---

## v1.2 (21-12-2023)

- Support for ownCloud 10.13.3
- Server URL display with non-standard ports
- Password visibility toggle options

---

## v1.1 (09-10-2023)

- Critical bug fix for incorrect client data
- Group deletion issue resolved during package changes
- Support for ownCloud 10.13.1.3
- 25 language translations added

---

## v1.0 (04-03-2023)

- First release
