# DevArt Image Gallery for Joomla

Professional image gallery component for Joomla 6, designed for editorial, news, magazine, and high-performance websites.

![Joomla](https://img.shields.io/badge/Joomla-6.x-blue)
![PHP](https://img.shields.io/badge/PHP-8.2%2B-green)
![Release](https://img.shields.io/badge/Version-1.0.11-orange)
![License](https://img.shields.io/badge/License-GPLv3-red)

---

## Overview

DevArt Image Gallery is a modern Joomla 6 gallery package built for stable image gallery management, legacy gallery compatibility, migration workflows, and lightweight frontend rendering.

It is designed for editorial, magazine, newspaper, portal, and high-traffic Joomla websites that need a clean, secure, reliable, and migration-friendly gallery workflow without unnecessary frontend bloat.

Version 1.0.11 introduces the new Thumbnail Cache system, significantly improving gallery performance by serving optimized thumbnails while preserving original gallery images.

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

### Thumbnail Cache System

New in Version 1.0.11

- Dedicated thumbnail cache architecture
- Separate thumbnail storage from original gallery images
- Per-gallery thumbnail settings
- Global default thumbnail settings
- Automatic thumbnail generation for newly uploaded images
- On-demand thumbnail generation for existing galleries
- Self-healing thumbnail regeneration
- Thumbnail cache versioning
- Automatic cleanup support
- High-traffic deployment friendly

Benefits:

- Faster gallery loading
- Reduced bandwidth consumption
- Smaller image payloads
- Better Core Web Vitals performance
- Improved Cloudflare and CDN efficiency

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
- CDN friendly
- Cloudflare friendly

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

- Homepage blocks
- Sidebars
- Landing pages
- Featured content areas

---

### Joomla Menu Item Integration

Create dedicated frontend gallery pages through Joomla menu items.

Ideal for:

- Standalone gallery pages
- Public gallery archives
- Visual landing pages
- Navigation-linked image collections

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
4. Thumbnails are generated automatically
5. Manage gallery photos
6. Insert gallery into article, module, or menu item
7. Publish

---

### For Existing Active Galleries

1. Upgrade to Version 1.0.11
2. No migration required
3. Thumbnail cache is created automatically when galleries are first accessed
4. Existing galleries continue to function normally

---

### For Legacy Migration

1. Configure Legacy Archive Directory
2. Rebuild Legacy Index
3. Verify indexed galleries
4. Continue using existing shortcodes
5. Thumbnail cache is created automatically only when galleries are requested

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

- Thumbnail cache system
- Lightweight frontend rendering
- Minimal JavaScript footprint
- Minimal CSS footprint
- No unnecessary frontend libraries
- Pagination for photo management
- Optimized query patterns
- Controlled indexing operations
- Joomla Page Cache friendly
- CDN friendly
- Cloudflare compatible
- High-traffic deployment friendly
- Progressive thumbnail generation
- Automatic thumbnail cache rebuilding
- Reduced frontend image payloads

---

## Compatibility Notes

Supported:

- Joomla 6.x
- PHP 8.2+
- Joomla native update system
- Modern Joomla MVC architecture

Not supported:

- Joomla 3
- Joomla 4
- Joomla 5
- Legacy PHP versions

---

## Current Version

1.0.11

---

## Changelog 1.0.11

### Added

- Thumbnail cache system
- Per-gallery thumbnail settings
- Global default thumbnail settings
- Dedicated thumbnail storage
- Automatic thumbnail generation
- On-demand thumbnail generation
- Missing thumbnail auto-rebuild
- Thumbnail cache retention controls
- Thumbnail cache versioning

### Improved

- Gallery frontend performance
- Bandwidth usage
- Cloudflare compatibility
- CDN efficiency
- Scalability for large galleries
- High-traffic deployment readiness

### Notes

- No database schema changes
- No migration required
- Existing galleries are not processed during upgrade
- Thumbnail cache is built progressively as galleries are accessed

---

## Production Recommendations

Recommended defaults:

Thumbnail Cache:

- Enabled
- WEBP format
- 400x350 thumbnails
- Crop mode
- 180-day retention

Frontend:

- Popup enabled
- Lazy loading enabled
- Responsive columns enabled
- Normal Grid or Masonry based on design

Uploads:

- Strict filename policy enabled
- Optimized output sizing
- Safe upload size limits

Migration:

- Use Legacy mode only for archive compatibility
- Use Active galleries for all new content

---

## Known Notes

- Existing Active and Legacy galleries build thumbnail cache only when first requested
- New gallery uploads generate thumbnails automatically
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
