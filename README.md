# DevArt Gallery for Joomla

Professional image gallery package for Joomla 6, designed for editorial, news, magazine, and high-performance websites.

![Joomla](https://img.shields.io/badge/Joomla-6.x-blue)
![PHP](https://img.shields.io/badge/PHP-8.3%2B-green)
![Release](https://img.shields.io/badge/Version-1.1.1-orange)
![License](https://img.shields.io/badge/License-GPLv3-red)

---

## Overview

DevArt Gallery is a modern Joomla 6 gallery package for stable image gallery management, legacy gallery compatibility, migration workflows, and lightweight frontend rendering.

It is designed for editorial, magazine, newspaper, portal, and high-traffic Joomla websites that need a clean, secure, reliable, and migration-friendly gallery workflow without unnecessary frontend bloat.

Version **1.1.1** builds on **1.1.0** with a Slider-style administrator Dashboard hub and expanded packaged languages (15 locales total).

Built specifically for Joomla 6 and PHP 8.3+.

---

## What's New in 1.1.1

- Administrator Dashboard rebuilt with Slider-style action cards (New Gallery, Galleries, Options)
- Galleries Index remains as a secondary action above stats and info panels
- Eight new packaged languages: Czech, Dutch, Polish, Russian, Ukrainian, Japanese, Turkish, Chinese (Simplified)
- Fifteen locales total (including Greek, French, German, Spanish, Italian, Portuguese, and English)
- Offline Argos translation pipeline with placeholder-safe gap fill

---

## What's New in 1.1.0

- Administrator Galleries, Index, and Dashboard rebuilt to match DevArt Widgets
- Gallery hub with Overview, Photos, and Settings tabs
- Packaged languages: Greek, French, German, Spanish, Italian, Portuguese
- Package-only update channel (`pkg_devartgallery`) at repository root
- Security, ACL, upload, path, and pagination hardening
- Frontend safety caps for module and content plugin image rendering

---

## Features

### Active Managed Galleries

- Create and manage galleries from the Joomla administrator
- Upload JPG, PNG, and WEBP images
- Automatic optimized image processing
- Configurable output quality and resizing
- Strict filename sanitization
- Manage Photos interface with pagination
- Scan Existing Photos support
- Optional per-gallery watermark support
- Automatic gallery image indexing
- Publishing state management

### Thumbnail Cache System

- Dedicated thumbnail cache architecture
- Separate thumbnail storage from original gallery images
- Per-gallery thumbnail settings with global defaults
- Automatic thumbnail generation for newly uploaded images
- On-demand thumbnail generation for existing galleries
- Thumbnail cache versioning and staged cleanup
- High-traffic and Cloudflare/CDN friendly

### Legacy Gallery Compatibility

- Read-only legacy gallery indexing
- Supports existing folder-based historical galleries
- Portable path-based gallery references
- Safe compatibility mode without modifying archive folders

### Shortcode Support

Legacy example:

`{gallery}oldgallery{/gallery}`

Active gallery examples:

`{gallery}galleries2/my-gallery{/gallery}`

`{devartgallery path="galleries2/my-gallery"}`

### Content Plugin, Editor Button, and Module

- Content plugin renders gallery shortcodes in articles
- Editor button inserts shortcodes from an indexed gallery picker
- Site module displays galleries in any module position
- Normal Grid and Masonry layouts
- Lightweight popup viewer
- Image limits with safety caps for large folders

### Menu Item Integration

Create dedicated frontend gallery pages through Joomla menu items with SEF-friendly routing.

---

## Included Extensions

Install the package only. Do not publish standalone extension ZIPs.

- `com_devartgallery` — administrator component and frontend gallery view
- `mod_devartgallery` — frontend gallery module
- `plg_content_devartgallery` — article shortcode renderer
- `plg_editors-xtd_devartgallery` — editor button for gallery insertion

All extensions update together through `pkg_devartgallery`.

---

## Requirements

- Joomla 6.0+
- PHP 8.3+

---

## Installation

1. Download `pkg_devartgallery_v1.1.1.zip` from [GitHub Releases](https://github.com/devartgr/joomla-devart-gallery/releases/tag/v1.1.1)
2. Go to `System → Install → Extensions`
3. Upload the package ZIP
4. Open `Components → DevArt Gallery`
5. Configure component options
6. Enable the content plugin, editor button plugin, and module if required

---

## Joomla Native Updates

DevArt Gallery uses Joomla native package updates only.

Update identity:

- Element: `pkg_devartgallery`
- Type: `package`

Update metadata:

- Update XML: https://raw.githubusercontent.com/devartgr/joomla-devart-gallery/main/update.xml
- Changelog: https://raw.githubusercontent.com/devartgr/joomla-devart-gallery/main/changelog.xml

Once installed, later updates appear under:

`System → Update → Extensions`

Existing sites on older releases should install the latest package ZIP once if needed. Later versions are found by Joomla Update.

---

## Recommended Workflow

### New Galleries

1. Configure Active Gallery Directory
2. Create a gallery and upload images
3. Thumbnails generate automatically on upload
4. Insert via article shortcode, module, or menu item

### Existing Active Galleries

1. Update to 1.1.1
2. No forced migration
3. Thumbnail cache builds on first frontend access if missing

### Legacy Migration

1. Configure Legacy Archive Directory
2. Rebuild Legacy Index
3. Keep existing shortcodes
4. Legacy galleries remain read-only in the administrator hub

---

## Security Highlights

- Joomla ACL permissions with custom actions
- CSRF protection for administrator actions
- Path traversal protection and hardened gallery path checks
- Upload size, dimension, and pixel-count validation
- Strict filename policy
- XSS-safe frontend rendering
- Keep Data on Uninstall option

---

## Performance

- Thumbnail cache system
- Lightweight frontend CSS/JS
- No jQuery or heavy frontend frameworks
- Pagination for photo management
- Controlled indexing operations
- Frontend image caps for module and content plugin
- Joomla Page Cache / Cloudflare friendly

---

## Compatibility

Supported:

- Joomla 6.x
- PHP 8.3+

Not supported:

- Joomla 3 / 4 / 5
- PHP 8.2 or earlier

---

## Current Version

**1.1.1**

Release: https://github.com/devartgr/joomla-devart-gallery/releases/tag/v1.1.1

Package SHA-256:

`1efc94d7ba5229c74e4800f67d7a645d5bc55ae41909dfa47e60c85359a145fe`

---

## Author

Kostas Stathopoulos — DevArt  
https://devart.gr

Repository: https://github.com/devartgr/joomla-devart-gallery

---

## Disclaimer / Limitation of Liability

This software is provided "as is", without warranty of any kind.

DevArt shall not be held liable for any damages, data loss, downtime, security issues, or other problems resulting from the use or misuse of this software.

Users are responsible for testing the software in their own environment and maintaining proper backups before installation or upgrades.

Always test on a staging environment before using in production.

---

## License

GNU General Public License version 3 or later
