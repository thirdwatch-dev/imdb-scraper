# IMDb Scraper

> Extract movie and TV show data, ratings, cast info, and reviews from IMDb

[![Try on Apify](https://img.shields.io/badge/Try_on-Apify_Store-00C853?style=for-the-badge)](https://apify.com/thirdwatch)
[![Website](https://img.shields.io/badge/Website-thirdwatch.dev-000?style=for-the-badge)](https://thirdwatch.dev)

## What it does

Scrapes IMDb for movie and TV show data including titles, ratings, cast and crew, genres, plot summaries, box office numbers, and user reviews. Supports search by title, genre, year, and IMDb top lists. The definitive source for entertainment industry data.

## Output fields

| Field | Type | Description |
|-------|------|-------------|
| title | String | Movie or TV show title |
| year | Number | Release year |
| rating | Number | IMDb rating (1-10) |
| votes | Number | Number of votes |
| genres | Array | Genre list |
| director | String | Director name |
| cast | Array | Main cast members |
| plot | String | Plot summary |
| runtime | String | Duration in minutes |
| boxOffice | Object | Gross earnings data |
| certificate | String | Age rating (PG, R, etc.) |
| imdbId | String | IMDb title ID |
| url | String | IMDb title URL |

## Input parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| queries | Array | Movie/show title search |
| genre | String | Genre filter |
| yearFrom | Number | Start year filter |
| yearTo | Number | End year filter |
| maxResults | Number | Maximum results per query |
| list | String | IMDb list (top250, popular, etc.) |

## Example output

```json
{
  "title": "Oppenheimer",
  "year": 2023,
  "rating": 8.4,
  "votes": 785432,
  "genres": ["Biography", "Drama", "History"],
  "director": "Christopher Nolan",
  "cast": ["Cillian Murphy", "Emily Blunt", "Matt Damon"],
  "plot": "The story of American scientist J. Robert Oppenheimer...",
  "runtime": "180 min",
  "boxOffice": {
    "budget": "$100,000,000",
    "worldwide": "$952,000,000"
  },
  "certificate": "R",
  "imdbId": "tt15398776",
  "url": "https://www.imdb.com/title/tt15398776/"
}
```

## Pricing

| Plan | Price |
|------|-------|
| Pay per result | $0.002/result |
| Free tier | Available on Apify |

## Use cases

- Entertainment industry market research
- Movie recommendation engine data collection
- Box office analysis and prediction modeling
- Film and TV content catalog building
- Academic research on cinema trends and ratings

## Getting started

1. Go to the [Apify Store](https://apify.com/thirdwatch)
2. Find the **IMDb Scraper**
3. Enter movie titles, genres, or browse lists
4. Run and download results as JSON, CSV, or Excel

## Related scrapers by Thirdwatch

- [Twitter Scraper](https://github.com/thirdwatch-dev/twitter-scraper) -- Social media data
- [Trustpilot Scraper](https://github.com/thirdwatch-dev/trustpilot-scraper) -- Reviews
- [Amazon Scraper](https://github.com/thirdwatch-dev/amazon-scraper) -- Product data
- [Google Maps Scraper](https://github.com/thirdwatch-dev/google-maps-scraper) -- Business data
- [Craigslist Scraper](https://github.com/thirdwatch-dev/craigslist-scraper) -- Classifieds

## About Thirdwatch

[Thirdwatch](https://thirdwatch.dev) builds production-ready web scraping APIs. 18 scrapers for jobs, e-commerce, reviews, social media, and business data.

## License

MIT
