# tori-tracker

A lightweight web application to manage, archive, and track secondhand listings across online marketplaces (such as Tori.fi, TechBBS, Vinted, Huuto.net, and Facebook Marketplace). Tikawe course work.

## The Problem
Selling items across multiple platforms makes it difficult to track where an item is currently listed, manage price histories, and monitor total annual sales revenue. When an item sells or an ad expires on a platform, its photos, descriptions, and price data are typically deleted or archived behind proprietary interfaces.

## The Solution
`tori-tracker` acts as an independent central ledger:
- Save listing drafts, descriptions, and live URLs in one place.
- Track active items across multiple selling venues.
- Record final sale prices, shipping fees, and profit margins.
- Aggregate annual revenue and profit metrics across all selling channels.

## Core Features
1. **User Accounts & Roles:** User registration, password hashing, and session management.
2. **Listing Inventory (CRUD):** Add, update, pause, and delete item listings.
3. **Platform Tracking:** Record active platforms (`tori`, `techbbs`, `vinted`, `huuto`, `fb`) with direct links to live listings.
4. **Categories & Tagging:** Assign items to multiple categories via a junction table.
5. **Search & Status Filtering:** Search by keywords across titles and descriptions; filter by status (`draft`, `active`, `paused`, `sold`) and platform.
6. **Peer Inquiries & Offers:** Allow other logged-in users to submit price offers or questions on active listings.
7. **Sales & Profit Analytics:** Aggregated statistics showing sold item counts, total gross sales, net margins, and alerts for listings active for over 30 days without updates.

## Current Status (Välipalautus 1)
Project repository initialized, data model defined, and core requirements specified. Development of the database schema and Flask backend is underway.

## Tech Stack
- **Backend:** Python 3, Flask
- **Database:** SQLite
- **Frontend:** Jinja2 templates, HTML5, minimal CSS

## Local Development Setup

### 1. Clone the repository
```bash
git clone git@github.com:tnli/tori-tracker.git
cd tori-tracker
