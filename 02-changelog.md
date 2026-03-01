# Changelog

### ownCloud module **[WHMCS](https://puqcloud.com/link.php?id=77)**
#####  [Order now](https://puqcloud.com/whmcs-module-owncloud.php) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-ownCloud/) | [FAQ](https://faq.puqcloud.com/)

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

- Module coded with ionCube v13
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
