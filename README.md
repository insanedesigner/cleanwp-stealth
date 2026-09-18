# CleanWP Stealth

### Clean. Control. Customize your WordPress footprint.

CleanWP Stealth is a lightweight WordPress plugin designed to reduce common public-facing WordPress fingerprints while providing useful endpoint controls and a customizable login URL.

It is built for agencies, developers, businesses, and website owners who want a cleaner and more controlled public-facing WordPress installation without modifying WordPress core.

---

## ✨ Features

### White-Label & Fingerprint Control

- Remove the WordPress generator fingerprint
- Remove common asset version query strings
- Remove RSD discovery tags
- Remove WLW manifest tags
- Remove WordPress shortlink tags
- Remove REST API discovery links

### Security & Endpoint Controls

- Disable XML-RPC when it is not required
- Protect public WordPress user REST endpoints
- Reduce basic user enumeration exposure
- Keep WordPress core untouched

### Custom Login URL

Use a custom login path instead of the standard WordPress login URL.

Example:

```text
https://example.com/wp-login.php

## 📋 Changelog

### 1.1.2 — Strict Login Protection

- Added strict protection for the default WordPress login endpoint.
- Direct requests to `/wp-login.php` now return HTTP 404 when Custom Login URL is enabled.
- Added protection against logged-out `/wp-admin/` requests.
- Logged-out `/wp-admin/` requests no longer redirect to the custom login URL.
- Prevented WordPress authentication redirects from exposing the custom login URL through `redirect_to`.
- Added protection for common alternative login/admin paths such as `/login/`, `/login.php`, `/admin/`, and `/dashboard/`.
- Preserved normal `/wp-admin/` functionality for authenticated administrators.
- Preserved `admin-ajax.php` and `admin-post.php` compatibility.
- Improved custom login endpoint handling.

### 1.1.1 — Custom Login & Admin UI Improvements

- Improved custom login URL routing.
- Added custom login URL settings interface.
- Added optional direct `wp-login.php` redirect control.
- Added protection status dashboard.
- Improved settings sanitization and output escaping.
- Added plugin settings shortcut.
- Improved activation and rewrite-rule handling.
- Added responsive administration interface.
- Added branded author and company information.
- Added Sudeep S / Sangamam Communications branding.
- Added plugin version information to the admin interface.
- Added recovery instructions for custom login URL configuration.

### 1.1.0 — Initial Enhanced Release

- Removed WordPress generator fingerprint.
- Added asset version fingerprint removal.
- Added RSD/WLW/shortlink/REST discovery cleanup.
- Added XML-RPC control.
- Added public user REST endpoint protection.
- Added optional WordPress sitemap control.
- Added custom login URL functionality.
- Added modern CleanWP Stealth administration interface.
- Added protection overview.
- Added configurable stealth controls.
- Added GPL-2.0-or-later licensing information.
- Added uninstall cleanup.
- Established Sudeep S as the plugin author.
- Established Sangamam Communications Pvt Ltd as the company behind the project.
