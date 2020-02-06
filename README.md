# cornholio
I wrote a notebook to scrape the Iowa Caucus results from https://results.thecaucuses.org

This was a little harder than scraping a regular table because it was a bunch of nested divs.  Even so, I was able to unwrap it pretty easily using beautifulsoup.

The result is a table with nested indexes in both the columns and the rows.  The columns are nested on candidate/type of vote count and the rows are nested on county/precinct.  Some libraries and programs don't like the multiindexes, so I also saved a version of the data with the row multiindex unwrapped.
