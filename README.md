# Web Scraper to extract hotel prices from Booking.com

Scraper to get Hotel price details from any search on Booking.com 

Full article at [ScrapeHero Tutorials](https://www.scrapehero.com/scrape-property-data-from-booking-com-using-google-chrome/)

## Usage

1. Install Requirements `pip3 install -r requirements.txt`
1. Search in Booking.com for Hotels 
1. Copy and add the search result URLS to [urls.txt](urls.txt)
1. Run `python3 scrape.py`
1. Get data from [data.csv](data.csv)

## Example Data Format

|name                                      |location                               |price |price_for        |room_type          |beds                  |rating|rating_title|number_of_ratings|url                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|------------------------------------------|---------------------------------------|------|-----------------|-------------------|----------------------|------|------------|-----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|Holiday Inn San Francisco - Golden Gateway|Nob Hill, San Francisco Show on map    |US$105|1 night, 2 adults|Standard  Room     |1 bed (1 large double)|8.0   |Very good   |1,087 reviews    |https://www.booking.com/hotel/us/holiday-inn-san-francisco-golden-gateway.en-gb.html?label=gen173nr-1DCAEoggI46AdIM1gEaKQCiAEBmAEJuAEHyAEM2AED6AEBiAIBqAIDuALCxJ31BcACAQ&sid=fd87930dc2332bf456ae77419c18c3a1&all_sr_blocks=18230001_251343373_0_2_0&checkin=2020-05-21&checkout=2020-05-22&dest_id=20015732&dest_type=city&group_adults=2&group_children=0&hapos=1&highlighted_blocks=18230001_251343373_0_2_0&hpos=1&no_rooms=1&sr_order=popularity&sr_pri_blocks=18230001_251343373_0_2_0__10500&srepoch=1588028809&srpvid=6d52a284d2ce0035&ucfs=1&from=searchresults ;highlight_room=#hotelTmpl|
|Handlery Union Square Hotel               |Union Square, San Francisco Show on map|US$99 |1 night, 2 adults|Petite Double Room |1 bed (1 double)      |8.2   |Very good   |2,278 reviews    |https://www.booking.com/hotel/us/handlery-union-square.en-gb.html?label=gen173nr-1DCAEoggI46AdIM1gEaKQCiAEBmAEJuAEHyAEM2AED6AEBiAIBqAIDuALCxJ31BcACAQ&sid=fd87930dc2332bf456ae77419c18c3a1&all_sr_blocks=5628504_245000754_0_0_0&checkin=2020-05-21&checkout=2020-05-22&dest_id=20015732&dest_type=city&group_adults=2&group_children=0&hapos=2&highlighted_blocks=5628504_245000754_0_0_0&hpos=2&no_rooms=1&sr_order=popularity&sr_pri_blocks=5628504_245000754_0_0_0__9900&srepoch=1588028809&srpvid=6d52a284d2ce0035&ucfs=1&from=searchresults ;highlight_room=#hotelTmpl                       |
|King George                               |Union Square, San Francisco Show on map|US$159|1 night, 2 adults|Superior Queen Room|1 bed (1 large double)|8.3   |Very good   |1,487 reviews    |https://www.booking.com/hotel/us/king-george.en-gb.html?label=gen173nr-1DCAEoggI46AdIM1gEaKQCiAEBmAEJuAEHyAEM2AED6AEBiAIBqAIDuALCxJ31BcACAQ&sid=fd87930dc2332bf456ae77419c18c3a1&all_sr_blocks=5625710_238956971_0_0_0&checkin=2020-05-21&checkout=2020-05-22&dest_id=20015732&dest_type=city&group_adults=2&group_children=0&hapos=3&highlighted_blocks=5625710_238956971_0_0_0&hpos=3&no_rooms=1&sr_order=popularity&sr_pri_blocks=5625710_238956971_0_0_0__15900&srepoch=1588028809&srpvid=6d52a284d2ce0035&ucfs=1&from=searchresults ;highlight_room=#hotelTmpl                                |
|The Pickwick Hotel San Francisco          |Union Square, San Francisco Show on map|US$139|1 night, 2 adults|Queen Room         |1 bed (1 large double)|7.3   |Good        |2,139 reviews    |https://www.booking.com/hotel/us/the-pickwick-san-francisco.en-gb.html?label=gen173nr-1DCAEoggI46AdIM1gEaKQCiAEBmAEJuAEHyAEM2AED6AEBiAIBqAIDuALCxJ31BcACAQ&sid=fd87930dc2332bf456ae77419c18c3a1&all_sr_blocks=5607711_190214860_0_0_0&checkin=2020-05-21&checkout=2020-05-22&dest_id=20015732&dest_type=city&group_adults=2&group_children=0&hapos=4&highlighted_blocks=5607711_190214860_0_0_0&hpos=4&no_rooms=1&sr_order=popularity&sr_pri_blocks=5607711_190214860_0_0_0__13900&srepoch=1588028809&srpvid=6d52a284d2ce0035&ucfs=1&from=searchresults ;highlight_room=#hotelTmpl                 |


## Learn More

This was not built for production deployments. There are several challenges for this simple scraper to work, when scraping a large number of pages. 


- [Scalable Large Scale Web Scraping – How to build, maintain and run scrapers](https://www.scrapehero.com/how-to-build-and-run-scrapers-on-a-large-scale/)
- [Web Scraping without getting Blocked](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)
## Disclaimer

Any code provided in our tutorials is for illustration and learning purposes only. We are not responsible for how it is used and assume no liability for any detrimental usage of the source code. The mere presence of this code on our repository does not imply that we encourage scraping or scrape the websites referenced in the code and accompanying tutorial. The tutorials only help illustrate the technique of programming web scrapers for popular internet websites. We are not obligated to provide any support for the code, however, if you add your questions in the comments section, we may periodically address them.
