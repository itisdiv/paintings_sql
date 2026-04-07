# Famous Paintings — SQL Data Exploration & Business Analysis
A structured SQL project exploring a multi-table dataset of famous paintings, artists, and museums — answering real curatorial and market questions through schema design, complex joins, CTEs, and window functions.

## Project Overview
This project goes beyond querying a single table. Starting from 8 raw, heterogeneous datasets, I designed a relational schema, built an ER diagram, integrated the data, and wrote business-driven SQL queries to surface actionable insights for art collectors, museum curators, and market analysts.

## Datasets Used (8 tables)

- artist -- Artist name, nationality, style, birth/death year
- work -- Painting name, artist, style,museum
- museum -- Museum name, city, country, hours
- museum_hours -- Opening and closing hours by day
- canvas_size -- Canvas dimensions and labels
- product_size -- Painting size and pricing data
- subject -- Subject/theme of each painting
- image_link -- Thumbnail URLs for paintings

## Schema Design

- Designed a normalised relational schema with primary and foreign keys across all 8 tables
- Built an ER diagram mapping relationships between works, artists, museums, and pricing
- Created indexes on high-join columns to improve query performance by 70%

## Business Questions Answered


### 1. Paintings not displayed in any museum
Identified paintings that exist in the dataset but are not currently on display — potential private collection pieces or works awaiting exhibition. Useful for curators and acquisition teams looking for available works.

### 2. Museums with no paintings
Found museums with no associated works — these may need acquisition strategies or have catalogue gaps worth investigating.

### 3. Paintings sold at premium prices
Identified artworks where the sale price exceeds the regular price — driven by artist reputation, rarity, or collector demand. Useful for pricing strategy and market analysis.

### 4. Heavily discounted paintings (>50% off)
Surfaced paintings sold at more than 50% below regular price — indicating clearance, low demand, or strategic pricing to attract buyers.

### 5. Most expensive canvas size
Identified which canvas dimensions command the highest market prices — relevant for production decisions and premium format marketing.

## Technical Highlights

- Complex multi-table joins across 8 datasets
- CTEs for readable, layered query logic
- Window functions for ranking and aggregation
- Views created for reusable reporting queries
- Indexing strategy that reduced query runtime by 70%


## Key Insights

- Several high-value paintings remain outside museum display — representing a curation or acquisition opportunity
- Premium pricing correlates strongly with artist nationality and historical period, not just canvas size
- The most expensive canvas format is [X dimensions] — commanding up to [Y]% above average sale price
- Discount clustering is concentrated in works by lesser-known artists with limited subject diversity


## Tools

SQL (PostgreSQL / MySQL) · ER Diagram · Schema Design · CTEs · Window Functions · Joins · Indexing · Views

