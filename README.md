# DevArt Gallery for Joomla

Professional image gallery component for Joomla 6, designed for editorial, news, and high-performance websites.

![Joomla](https://img.shields.io/badge/Joomla-6.x-blue)
![PHP](https://img.shields.io/badge/PHP-8.2%2B-green)
![Release](https://img.shields.io/badge/Version-1.0.0-orange)
![License](https://img.shields.io/badge/License-GPLv3-red)

---

## Overview

DevArt Gallery is a modern Joomla 6 gallery package built for stable image gallery management, legacy gallery compatibility, and lightweight frontend rendering.

It is designed for editorial and high-traffic Joomla websites that need a clean, secure, and reliable gallery workflow without unnecessary frontend bloat.

---

## Features

### Active Galleries

- Create and manage new galleries from the Joomla administrator
- Upload JPG, PNG and WEBP images
- Automatic optimized JPG output workflow
- Strict filename sanitization
- Manage Photos interface
- Pagination support for larger galleries
- Scan Existing Photos support
- Optional watermark support
- Gallery image count indexing

### Legacy Galleries

- Read-only legacy gallery indexing
- Supports existing folder-based galleries
- Useful for migrations and long-running Joomla websites
- No forced ID-based gallery migration
- Keeps historical gallery paths portable across sites

### Shortcodes

DevArt Gallery supports simple article shortcodes:

`{gallery}galleryname{/gallery}`

`{gallery}galleries2/galleryname{/gallery}`

This allows both legacy and active galleries to work with clean path-based references.

### Content Plugin

- Renders gallery shortcodes inside Joomla articles
- Supports multiple galleries per article
- Lightweight frontend output
- Compatible with Joomla Page Cache and CDN environments

### Editor Button

- Insert gallery shortcodes directly from the Joomla editor
- Gallery picker for easier article workflow
- Helps editors avoid manual shortcode typing

### Frontend Module

- Display selected galleries in module positions
- Normal gallery layout support
- Popup viewer support
- Useful for sidebars, homepage blocks, and custom layouts

### Popup Viewer

- Lightweight popup image viewer
- No heavy external gallery framework
- No image filename caption by default
- Designed to avoid template conflicts

---

## Included Extensions

This package installs:

- com_devartgallery
- mod_devartgallery
- plg_content_devartgallery
- plg_editors-xtd_devartgallery

---

## Requirements

- Joomla 6.x
- PHP 8.2+

---

## Installation

1. Download the latest release from GitHub
2. Go to System → Extensions → Install
3. Upload the package zip file
4. Open Components → DevArt Gallery
5. Configure Options
6. Enable the content plugin, editor button plugin, and module if needed

---

## Joomla Updates

DevArt Gallery supports Joomla's native update system via GitHub.

Once installed, future updates will be available via:

System → Extensions → Update

Update server:

`https://raw.githubusercontent.com/devartgr/joomla-devart-gallery/main/update.xml`

---

## Recommended Workflow

1. Configure active and legacy gallery base folders
2. Rebuild the gallery index when importing existing folders
3. Create new galleries from the DevArt Gallery administrator interface
4. Upload images through Manage Photos
5. Insert galleries into articles using the editor button or shortcode
6. Use the module for homepage or sidebar gallery display

---

## Security Highlights

- Joomla ACL permissions support
- CSRF protection for administrator actions
- SQL injection protection through Joomla database APIs
- XSS protection with escaped output
- Path traversal protection for filesystem operations
- Strict filename policy for safer uploads
- GPL licensed and JED-ready packaging

---

## Performance

- Lightweight frontend rendering
- Minimal JavaScript and CSS footprint
- No unnecessary external libraries
- Pagination for photo management
- Optimized query patterns
- Controlled batch operations
- Joomla Page Cache friendly
- Cloudflare/CDN friendly
- Designed for high-traffic production environments

---

## Compatibility Notes

DevArt Gallery is built only for modern Joomla environments.

Supported:

- Joomla 6.x
- PHP 8.2+
- Modern Joomla MVC architecture
- Joomla native update system

Not supported:

- Joomla 3
- Joomla 4
- Joomla 5
- Legacy PHP versions

---

## Current Version

1.0.0

---

## Changelog 1.0.0

- First production release for Joomla 6
- Added modern Joomla 6 MVCComponent architecture
- Added service provider integration
- Added active gallery management
- Added legacy gallery read-only indexing
- Added shortcode rendering through content plugin
- Added editor button integration
- Added frontend gallery module
- Added popup viewer
- Added Manage Photos pagination
- Added Scan Existing Photos support
- Added strict filename policy
- Added JPG, PNG and WEBP upload support
- Added optional watermark support
- Added Joomla ACL support
- Added Keep Data on Uninstall option
- Added GitHub-based Joomla update support
- Added JED-ready GPL metadata and PHP license notices

---

## Known Notes

- Editor button gallery ordering may receive further refinements in a future update
- Always test gallery rendering with the active Joomla template and cache setup before full production rollout

---

## Author

Kostas Stathopoulos  
DevArt  
https://devart.gr/

---

## Disclaimer / Limitation of Liability

This software is provided "as is", without warranty of any kind.
DevArt shall not be held liable for any damages, data loss, downtime,
security issues, or other problems resulting from the use or misuse
of this software.

Users are responsible for testing the software in their own environment
and maintaining proper backups before installation or upgrades.

Always test on a staging environment before using in production.

---

## License

GNU General Public License v3 or later
