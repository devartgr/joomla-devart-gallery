# DevArt Image Gallery for Joomla

Professional image gallery component for Joomla 6, designed for editorial, news, magazine, and high-performance websites.

![Joomla](https://img.shields.io/badge/Joomla-6.x-blue)
![PHP](https://img.shields.io/badge/PHP-8.2%2B-green)
![Release](https://img.shields.io/badge/Version-1.0.9-orange)
![License](https://img.shields.io/badge/License-GPLv3-red)

---

## Overview

DevArt Image Gallery is a modern Joomla 6 gallery package built for stable image gallery management, legacy gallery compatibility, migration workflows, and lightweight frontend rendering.

It is designed for editorial, magazine, and high-traffic Joomla websites that need a clean, secure, reliable, and migration-friendly gallery workflow without unnecessary frontend bloat.

---

## Features

### Active Managed Galleries

- Create and manage new galleries directly from the Joomla administrator
- Upload JPG, PNG and WEBP images
- Automatic optimized image processing
- Configurable output quality and resizing
- Strict filename sanitization
- Manage Photos interface
- Pagination support for larger galleries
- Scan Existing Photos support
- Optional per-gallery watermark support
- Automatic gallery image indexing
- Publishing state management

---

### Legacy Gallery Compatibility

- Read-only legacy gallery indexing
- Supports existing folder-based historical galleries
- Ideal for migrations from older Joomla gallery workflows
- No forced ID-based migration
- Portable path-based gallery references
- Safe compatibility mode without modifying archive folders

---

### Shortcode Support

DevArt Image Gallery supports portable article shortcodes.

Legacy example:

`{gallery}oldgallery{/gallery}`

Active gallery example:

`{gallery}galleries2/my-gallery{/gallery}`

This allows clean migration-friendly gallery publishing across Joomla installations.

---

### Joomla Content Plugin

- Renders gallery shortcodes directly inside Joomla articles
- Supports multiple galleries in a single article
- Lightweight frontend rendering
- Joomla Page Cache compatible
- CDN / Cloudflare friendly output

---

### Editor Button Integration

- Native Joomla editor button
- Gallery picker popup
- Fast shortcode insertion
- Cleaner editorial workflow
- No manual shortcode typing required

---

### Frontend Module

Display galleries anywhere using Joomla module positions.

Features:

- Gallery selector
- Normal Grid layout
- Masonry layout
- Popup viewer support
- Image limits
- Access control support
- Menu assignment support

Ideal for:

- homepage blocks
- sidebars
- landing pages
- featured content areas

---

### Joomla Menu Item Integration

Create dedicated frontend gallery pages through Joomla menu items.

Ideal for:

- standalone gallery pages
- public gallery archives
- visual landing pages
- navigation-linked image collections

---

### Popup Viewer

- Lightweight popup image viewer
- No heavy external gallery frameworks
- Responsive behavior
- Optional frontend popup mode
- No filename captions by default
- Designed to minimize template conflicts

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
2. Go to:

`System → Extensions → Install`

3. Upload the package ZIP file
4. Open:

`Components → DevArt Image Gallery`

5. Configure component options
6. Enable the content plugin, editor button plugin, and module if required

---

## Joomla Native Updates

DevArt Image Gallery supports Joomla native updates via GitHub.

Once installed, future updates are available through:

`System → Extensions → Update`

Update server:

`https://raw.githubusercontent.com/devartgr/joomla-devart-gallery/main/update.xml`

---

## Recommended Workflow

### For New Galleries

1. Configure Active Gallery Directory
2. Create a new gallery
3. Upload images
4. Manage gallery photos
5. Insert gallery into article, module, or menu item
6. Publish

---

### For Legacy Migration

1. Configure Legacy Archive Directory
2. Rebuild Legacy Index
3. Verify indexed galleries
4. Continue using existing shortcodes

---

## Security Highlights

- Joomla ACL permissions support
- CSRF protection for administrator actions
- SQL injection protection through Joomla database APIs
- XSS-safe frontend rendering
- Path traversal protection
- Strict filename policy
- Safe legacy archive compatibility
- GPL licensed
- JED-ready packaging

---

## Performance

Built for production environments.

Features include:

- lightweight frontend rendering
- minimal JavaScript footprint
- minimal CSS footprint
- no unnecessary frontend libraries
- pagination for photo management
- optimized query patterns
- controlled indexing operations
- Joomla Page Cache friendly
- CDN friendly
- Cloudflare compatible
- high-traffic deployment friendly

---

## Compatibility Notes

Supported:

- Joomla 6.x
- PHP 8.2+
- Joomla native update system
- modern Joomla MVC architecture

Not supported:

- Joomla 3
- Joomla 4
- Joomla 5
- legacy PHP versions

---

## Current Version

1.0.9

---

## Changelog 1.0.9

- Fixed Joomla component configuration parameter handling when stored in nested JSON format
- Fixed Dashboard showing fallback or incorrect gallery paths instead of configured values
- Fixed Legacy Archive Directory display inconsistencies
- Fixed Active Gallery Directory display inconsistencies
- Fixed Legacy Index rebuild using incorrect directory values in specific installations
- Fixed Active Index rebuild using incorrect directory values in specific installations
- Fixed indexing behavior when configuration values were correctly saved but incorrectly read
- Improved compatibility with different Joomla parameter storage behaviors
- Improved gallery indexing reliability
- Improved migration safety
- Improved internal configuration loading consistency

---

## Production Recommendations

Recommended defaults:

Frontend:

- Popup enabled
- Lazy loading enabled
- Responsive columns enabled
- Normal Grid or Masonry based on design

Uploads:

- strict filename policy enabled
- optimized output sizing
- safe upload size limits

Migration:

- use Legacy mode only for archive compatibility
- use Active galleries for all new content

---

## Known Notes

- Editor button gallery ordering may receive further refinements in a future update
- Always test template compatibility and caching behavior before full production rollout

---

## Author

Kostas Stathopoulos  
DevArt  
https://devart.gr/

GitHub Repository:

https://github.com/devartgr/joomla-devart-gallery

---

## Disclaimer / Limitation of Liability

This software is provided "as is", without warranty of any kind.

DevArt shall not be held liable for any damages, data loss, downtime, security issues, or other problems resulting from the use or misuse of this software.

Users are responsible for testing the software in their own environment and maintaining proper backups before installation or upgrades.

Always test on a staging environment before using in production.

---

## License

GNU General Public License v3 or later
