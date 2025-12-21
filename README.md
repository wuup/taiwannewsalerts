# Taiwan News Alerts

Static news site for Taiwan Strait security intelligence, built with Jekyll and hosted on GitHub Pages.

## Features

- Dark theme matching [Taiwan Invasion Alerts](https://taiwaninvasionalerts.com)
- Daily briefing posts auto-generated from TIA events
- Categorized by severity (critical, intel, routine, news)
- Mobile-responsive design

## Local Development

```bash
bundle install
bundle exec jekyll serve
```

## Generate Daily Posts

```bash
# Generate yesterday's post
python scripts/generate_daily_post.py

# Backfill last N days
python scripts/generate_daily_post.py --backfill 20

# Specific date
python scripts/generate_daily_post.py --date 2025-12-15
```

## Deployment

Automatically deployed to GitHub Pages on push to main branch.

Live at: https://wuup.github.io/taiwannewsalerts/
