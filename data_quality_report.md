# Unified Books Dataset — Data Quality Report
Generated: 2026-11-08

Total records: 57,332  
Unique `book_id` values: 57,332

## Cleaning performed

- Repaired 80 ISBN values with a numeric `.0` suffix, preserving ISBNs ending in `X`.
- Normalized 7 `ebook` format values to `Ebook`.
- Marked the single `UNKNOWN` title as missing rather than treating it as a valid title.
- Serialized integer-valued year, page, rating-count, and review-count fields without `.0` suffixes, retaining blanks for missing values.
- Removed no rows: there were no exact duplicate rows or values outside the checked numeric ranges.
- Did not impute missing bibliographic metadata because the dataset does not provide evidence for inferred values.

## Records by source

| Source | Records |
|---|---:|
| `openlibrary_books` | 55,993 |
| `goodreads_books_dataset` | 903 |
| `prog_book` | 271 |
| `best_selling_books` | 165 |

## Missing values by column

| Column | Missing |
|---|---:|
| `book_id` | 0 |
| `title` | 1 |
| `subtitle` | 55,572 |
| `series_name` | 56,924 |
| `series_position` | 56,939 |
| `authors` | 1,904 |
| `description` | 56,207 |
| `genres` | 235 |
| `language` | 7,241 |
| `format` | 43,286 |
| `first_published_year` | 1,451 |
| `publication_date` | 56,466 |
| `pages` | 56,272 |
| `rating` | 56,187 |
| `ratings_count` | 56,429 |
| `reviews_count` | 56,158 |
| `price_usd` | 57,061 |
| `isbn` | 56,652 |
| `thumbnail_url` | 30,889 |
| `source_url` | 436 |
| `sample_review` | 56,543 |
| `source_dataset` | 0 |
| `source_record_id` | 0 |
| `date_ingested` | 0 |
| `approx_sales_millions` | 57,167 |

## Numeric field summary

| Field | Count | Mean | Std. dev. | Min | 25% | Median | 75% | Max |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| `first_published_year` | 55,881 | 2003.505628 | 30.284950 | 1304 | 2000 | 2014 | 2020 | 2026 |
| `pages` | 1,060 | 441.966038 | 574.984988 | 1 | 224 | 347 | 467.75 | 10,358 |
| `rating` | 1,145 | 3.937223 | 0.395968 | 1 | 3.75 | 3.95 | 4.18 | 5 |
| `ratings_count` | 903 | 159,813.1 | 612,467.6 | 0 | 102.5 | 3,966 | 65,457 | 9,799,364 |
| `reviews_count` | 1,174 | 60.011073 | 273.891879 | 0 | 9 | 30 | 30 | 5,938 |
| `price_usd` | 271 | 54.541860 | 35.711485 | 9.323529 | 30.751471 | 46.317647 | 67.854412 | 235.65 |
| `approx_sales_millions` | 165 | 29.138788 | 25.392232 | 10 | 13 | 20 | 36 | 200 |

## Repeated titles

There are 2,898 repeated non-missing title groups. Of those, 2,764 groups contain more than one author (9,451 records). These were retained because matching titles do not establish that records are duplicates.
