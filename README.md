I've always been fustrated by how so much "open" data covers very short time periods. Understanding a snapshot of something is useful, but one can have little context as to variance and signifigance without a little bit more history - ie data that measures multiple cycles and "epochs."


Here I attempt to get as much history at a granular level for transit ridership. I expect to build this out over time.

To often when the data is avaliable it is in some horrible PDF or website form. I plan on standardizing formats and getting everything into CSV and JSON objects.

For now I'm investing in:
1) New York City Subway station level data
2) Amtrak station level data

I'm breaking up the data with folders by region and system. I'll include data dictionaries and little gottcha mentioned in README's for each system.

Each folder is structured as:
- raw: the data in it's rawest form: pdfs, saved webpages, pictures from books etc. Nothing will have been done to this data other then finding a way to save/store the data
- cleaned: this data will be manipulated in some way from the raw, almost always just getting the data into CSV or JSON form. Some light enrichment can also occur here
- transform: not always used, but transform will have much more heavily manipulated/assumption driven work in. Filling in missing data, matching up not exactly matching data, fuzzy joins, analytical outputs etc
workflow: the logic behind transformations from raw > cleaned > transform
- canonical: this is where you go if you want to get the latest and greatest version of the data. You'll also find the data dictionary in here in JSON form.
- analysis: what it sounds like. getting conclusions from the data

