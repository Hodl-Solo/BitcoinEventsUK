# UK Bitcoin Meetups - Simplified Website Plan

## Overview
A simple, fast, static HTML site listing all UK & Ireland Bitcoin meetups.

## Hosting
- **Cloudflare Pages** - Free, global CDN, custom domain

## Site Structure

### Single Page Option
```
index.html - All meetups on one page, grouped by day/region
```

### Sections
1. **Header** - Site title + tagline
2. **About** - Brief description (1-2 sentences)
3. **Meetups by Day** - All meetups grouped by day of week
4. **Meetups by Region** - All meetups grouped by region (optional)
5. **Footer** - Links to newsletter, contact, Nostr

## Data Structure (Static JSON)
```json
{
  "meetups": [
    {
      "name": "London Bitcoin Space",
      "location": "London",
      "day": "Wednesday",
      "time": "18:30",
      "venue": "The Gallery",
      "address": "...",
      "website": "https://...",
      "nostr": "npub1...",
      "twitter": "...",
      "telegram": "..."
    }
  ]
}
```

## Content to Include
- Meetup name
- Location/City
- Day of week (or date)
- Time
- Venue name + address
- Links (Website, Nostr, Twitter, Telegram)
- Brief description (optional)

## Design Goals
- **Fast** - Static HTML, no database
- **Simple** - Easy to update (just edit JSON/HTML)
- **Mobile-friendly** - Works on phones
- **No bloat** - No plugins, no CMS, no tracking
