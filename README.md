# The Worldworthy 100 — 2026 open dataset

## What this is

The 2026 edition of The Worldworthy 100: the world's 100 best in every category, ranked by consensus. This release contains 43 currently published lists (33 venue lists and 10 city lists), with 100 ranked entries each: 4,300 rows in `all_rankings.csv`. Each ranking also has its own CSV. Rank is meaningful within its own list, not as a comparison across categories.

Only complete, live-published rankings are included. Hotels, wellness hotels and all company rankings are excluded. Incomplete and unpublished rankings are not included. This export does not calculate, filter or reorder rankings.

## Files and columns

Every CSV has exactly these seven columns, in order:

`list,rank,name,city,country,worldworthy_score,page_url`

- `list`: the published category slug.
- `rank`: the existing position, from 1 to 100 within that list.
- `name`: the name displayed on the live list.
- `city`: the source CSV city, or empty when unspecified. City rankings also retain an empty city field when that is how the source represents them; the city's name is in `name`.
- `country`: the source CSV country.
- `worldworthy_score`: the public final Worldworthy Score, displayed to two decimals and capped at 9.99, matching the live entry. It is not a raw platform rating. Scores should be interpreted within their own category.
- `page_url`: the exact canonical pathname from the live list's generated ItemList; prepend `https://worldworthy.org` to open it.

CSV files are UTF-8, comma-delimited, with a header and LF line endings. `datapackage.json` supplies Frictionless metadata, field types, constraints, file sizes and SHA-256 checksums. The combined file repeats the per-list rows; do not count both as separate observations.

Only the seven listed fields are distributed: no raw platform ratings, review counts, third-party review text, contact details, addresses, images or quotations are included.

## Methodology

The Worldworthy Index ranks by consensus: what visitors report across platforms, recognition in international guides and the press, and public and professional records. Evidence is calibrated by category and country. Eligibility, operating status and duplicates are checked, and an editor reviews each list before publication. No venue can apply or pay to be listed.

City lists are computed from each city's ranked-eligible entries and measured within size tiers, so a town is measured against towns and a capital against capitals. Geographic limits keep rankings global. Israel, where the publisher is based, is not ranked in the 2026 edition. These rankings describe visitor experience, not an inspection or a guarantee of quality, safety or availability. See the [published methodology](https://worldworthy.org/methodology/) for context; proprietary weighting is not distributed in this dataset.

## The lists

The introductions below are taken from the approved list definitions in `build_site.py`.

### Airports

`airports.csv` — [Live list](https://worldworthy.org/lists/airports/)

Airports, ranked by the passengers who pass through them.

### Archaeological Sites

`archaeological-sites.csv` — [Live list](https://worldworthy.org/lists/archaeological-sites/)

Ruins and excavations open to visitors.

### Bakeries

`bakeries.csv` — [Live list](https://worldworthy.org/lists/bakeries/)

Bread first.

### BBQ Smokehouses

`bbq-smokehouses.csv` — [Live list](https://worldworthy.org/lists/bbq-smokehouses/)

Smokehouses outside the United States.

### Beaches

`beaches.csv` — [Live list](https://worldworthy.org/lists/beaches/)

Public beaches, ranked by what their visitors keep coming back for.

### Botanical Gardens

`botanical-gardens.csv` — [Live list](https://worldworthy.org/lists/botanical-gardens/)

Gardens built around plants, from glasshouses to arboretums.

### Breweries

`breweries.csv` — [Live list](https://worldworthy.org/lists/breweries/)

Breweries with a taproom or visits.

### Brunch & Breakfast

`brunch-breakfast.csv` — [Live list](https://worldworthy.org/lists/brunch-breakfast/)

Where the morning is the point.

### Burgers

`burgers.csv` — [Live list](https://worldworthy.org/lists/burgers/)

Burger restaurants, not chains.

### Cable Cars

`cable-cars.csv` — [Live list](https://worldworthy.org/lists/cable-cars/)

Cable cars, gondolas, funiculars and cog railways.

### Canyons & Gorges

`canyons-gorges.csv` — [Live list](https://worldworthy.org/lists/canyons-gorges/)

Canyons and gorges you can reach.

### Castles & Fortresses

`castles.csv` — [Live list](https://worldworthy.org/lists/castles/)

Castles, fortresses and citadels.

### Cocktail Bars

`cocktail-bars.csv` — [Live list](https://worldworthy.org/lists/cocktail-bars/)

Bars built around the cocktail.

### Coffee Houses

`coffee-houses.csv` — [Live list](https://worldworthy.org/lists/coffee-houses/)

Cafés where the coffee is the point.

### Food Markets

`food-markets.csv` — [Live list](https://worldworthy.org/lists/food-markets/)

Covered and open-air markets with food stalls.

### Football Stadiums

`football-stadiums.csv` — [Live list](https://worldworthy.org/lists/football-stadiums/)

Stadiums where football is played.

### Hikes

`hikes.csv` — [Live list](https://worldworthy.org/lists/hikes/)

Named trails with a start point, from an afternoon walk to a multi-day route.

### Ice Cream Parlours

`ice-cream.csv` — [Live list](https://worldworthy.org/lists/ice-cream/)

Gelato, ice cream, kulfi and dondurma shops, ranked by the people who queue for them.

### Kebab & Döner

`kebab-doner.csv` — [Live list](https://worldworthy.org/lists/kebab-doner/)

Kebab, döner, shawarma and gyros shops.

### Landmarks

`landmarks.csv` — [Live list](https://worldworthy.org/lists/landmarks/)

Monuments, towers, bridges, squares, stations and natural landmarks.

### Most Beautiful Cities

`most-beautiful-cities.csv` — [Live list](https://worldworthy.org/lists/most-beautiful-cities/)

Beaches, parks, gardens, palaces, landmarks and the countryside around them.

### Most Beautiful Cities in Europe

`most-beautiful-cities-europe.csv` — [Live list](https://worldworthy.org/lists/most-beautiful-cities-europe/)

The European cities whose nature and architecture visitors rate highest.

### Most Charming Towns & Small Cities

`most-charming-cities.csv` — [Live list](https://worldworthy.org/lists/most-charming-cities/)

Municipalities of 5,000 to 300,000 residents that visitors rate like capitals.

### Most Delicious Cities

`most-delicious-cities.csv` — [Live list](https://worldworthy.org/lists/most-delicious-cities/)

The cities visitors love to eat in: pizza, ramen, ice cream, coffee, bakeries, markets and more.

### Most Loved Cities

`most-loved-cities.csv` — [Live list](https://worldworthy.org/lists/most-loved-cities/)

The cities visitors love most, measured from the city’s ranked-eligible entries across the Worldworthy 100 lists.

### Most Loved Cities in the Americas

`most-loved-cities-americas.csv` — [Live list](https://worldworthy.org/lists/most-loved-cities-americas/)

The cities of North, Central and South America that visitors love most, measured from the city’s ranked-eligible entries across the Worldworthy 100 lists.

### Most Loved Cities in Asia-Pacific

`most-loved-cities-asia-pacific.csv` — [Live list](https://worldworthy.org/lists/most-loved-cities-asia-pacific/)

The cities of Asia and Oceania that visitors love most, measured from the city’s ranked-eligible entries across the Worldworthy 100 lists.

### Most Loved Cities in Europe

`most-loved-cities-europe.csv` — [Live list](https://worldworthy.org/lists/most-loved-cities-europe/)

The European cities visitors love most, measured from the city’s ranked-eligible entries across the Worldworthy 100 lists.

### Most Worldworthy Cities

`most-worldworthy-cities.csv` — [Live list](https://worldworthy.org/lists/most-worldworthy-cities/)

The cities with the most Laureates across every Worldworthy 100 list.

### Museums

`museums.csv` — [Live list](https://worldworthy.org/lists/museums/)

Museums of every kind, open to the public, ranked by what visitors say about their visit, not by the size of the collection.

### Palaces

`palaces.csv` — [Live list](https://worldworthy.org/lists/palaces/)

Palaces open to visitors.

### Parks

`parks.csv` — [Live list](https://worldworthy.org/lists/parks/)

City and landscape parks, not national parks.

### Pastry Shops

`pastry-shops.csv` — [Live list](https://worldworthy.org/lists/pastry-shops/)

Patisseries, confectioners and dessert shops.

### Pizzerias

`pizzerias.csv` — [Live list](https://worldworthy.org/lists/pizzerias/)

Pizzerias, not Italian restaurants that also serve pizza.

### Ramen

`ramen-shops.csv` — [Live list](https://worldworthy.org/lists/ramen-shops/)

Ramen and tsukemen shops on five continents.

### Rising Cities

`rising-cities.csv` — [Live list](https://worldworthy.org/lists/rising-cities/)

Cities of 20,000 residents or more whose eligible entries are rated above the global mean while carrying fewer than 150,000 reviews in total: loved by the visitors who have found them, not yet famous.

### Saunas & Baths

`saunas-baths.csv` — [Live list](https://worldworthy.org/lists/saunas-baths/)

Public bathing with a day ticket: thermal baths, hot springs, onsen, hammams and banyas.

### Shopping Malls

`shopping-malls.csv` — [Live list](https://worldworthy.org/lists/shopping-malls/)

Malls, shopping centres, historic arcades and outlet villages.

### Show Caves

`show-caves.csv` — [Live list](https://worldworthy.org/lists/show-caves/)

Caves open to visitors with tours, lights and a path.

### Theme Parks

`theme-parks.csv` — [Live list](https://worldworthy.org/lists/theme-parks/)

Amusement parks; water-only parks excluded.

### Waterfalls

`waterfalls.csv` — [Live list](https://worldworthy.org/lists/waterfalls/)

Waterfalls you can reach, from roadside giants to a day’s hike.

### Wineries

`wineries.csv` — [Live list](https://worldworthy.org/lists/wineries/)

Wineries and cellars open to visitors, ranked by what visitors say about the visit, not by the wine in the glass.

### Zoos & Aquariums

`zoos-aquariums.csv` — [Live list](https://worldworthy.org/lists/zoos-aquariums/)

Zoos and aquariums.

## Citation

The Worldworthy 100, 2026, worldworthy.org

When reusing a subset, also link to the relevant live list or entry and indicate any changes you make.

## License and contact

This dataset is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). Attribution is required. See `LICENSE.md`.

Publisher: Worldworthy. Contact: press@worldworthy.org.
