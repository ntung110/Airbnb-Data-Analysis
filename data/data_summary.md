# Data Summary

> Provde a summary of features in the three datasets as well as the expected feature type

## General Info
- `listings.csv`: Detailed information about the listings, including location, host information, pricing and ratings

- `calendar.csv`: Detailed information about daily availability and pricing in the last 12 months

- `reviews.csv`: Reviews of bookers who have stayed at the listings

## Listings Dataset Summary

### Listing Information
- `id` &rarr;  `int`: ID of listings 

- `listing_url` &rarr; `object`: URL of listing
- `scrape_id` &rarr; `int`: ID of listing specified by the scraper
- `last_scraped` &rarr; `datetime`: Last date that the data was scraped
- `source` &rarr; `object`: Source of scraped data
- `name` &rarr; `object`: Name of property listed
- `description` &rarr; `object`: Description of listing
- `neighbourhood_overview` &rarr; `object`: Description of neighbourhood of listing
- `picture_url` &rarr; `object`: URL of pictures included in the listing

### Host Information
- `host_id` &rarr; `int`: ID of host

- `'host_url'` &rarr; `object`: URL of host's profile
- `host_name` &rarr; `object`: Name of host
- `host_since` &rarr; `datetime`: Date when host started on Airbnb
- `host_location` &rarr; `object`: Location of host
- `host_about` &rarr; `object`: Contents in the host's introduction
- `host_response_time` &rarr; `object`: Typical response time from the host
- `host_response_rate` &rarr; `float`: Typical response rate from the host
- `host_acceptance_rate` &rarr; `float`: Typical acceptance rate from the host
- `host_is_superhost` &rarr; `bool`: Indicator of whether host is a superhost
- `host_thumbnail_url` &rarr; `object`: URL of host's thumbnail 
- `host_picture_url` &rarr; `object`: URL of host's profile picture 
- `host_neighbourhood` &rarr; `object`: Neighbourhood of host
- `host_listings_count` &rarr; `int`: The number of active listings the host has (Airbnb calculations)
- `host_total_listings_count` &rarr; `int`: The number of listings total the host has listed from the past until present (Airbnb calculations)
- `host_verifications` &rarr; `list[object]`: Methods of verication that the host has signed up
- `host_has_profile_pic` &rarr; `bool`: Indicator of whether host has a profile picture
- `host_identity_verified` &rarr; `bool`: Indicator of whether host has been verified by Airbnb

### Geographical Information
- `neighbourhood` &rarr; `object`: Specific neighbourhood where property is located by Airbnb (inaccurate)

- `neighbourhood_cleansed` &rarr; `object`: Specific neighbourhood where property is located according to public datafiles
- `neighbourhood_group_cleansed` &rarr; `object`: Broad geographical area where property is located according to public datafiles
- `latitude` &rarr; `float`: Latitude position of property listed
- `longitude` &rarr; `float`: Longitude position of property listed

### Property Information
- `property_type` &rarr; `object`: Self-selected property type

- `room_type` &rarr; `object`: Type of room offered in listings [Entire home/apt | Private room | Shared room | Hotel]
- `accommodates` &rarr; `int`: Maximum number of occupations possible in the property
- `bathrooms` &rarr; `int`: Number of bathrooms in the listings
- `bathrooms_text` &rarr; `object`: Number of bathrooms represented as text
- `bedrooms` &rarr; `int`: Number of bedrooms in the listings
- `beds` &rarr; `int`: Number of beds
- `amenities` &rarr; `list[object]`: Ammenities available in the property
- `price` &rarr; `float`: Price of listings
- `minimum_nights` &rarr; `int`: Minimum number of nights stayed for the listings
- `maximum_nights` &rarr; `int`: Maximum number of nights stayed for the listings
- `minimum_minimum_nights` &rarr; `int`: Smallest minimum_night value in the next 365 days
- `maximum_minimum_nights` &rarr; `int`: Largest minimum_night value in the next 365 days
- `minimum_maximum_nights` &rarr; `int`: Smallest maximum_night value in the next 365 days
- `maximum_maximum_nights` &rarr; `int`: Largest maximum_night value in the next 365 days
- `minimum_nights_avg_ntm` &rarr; `float`: Average minimum nights value in the next 365 days
- `maximum_nights_avg_ntm` &rarr; `float`: Average maximum nights value in the next 365 days
- `calendar_updated` &rarr; `datetime`: Date when the calendar was last updated 
- `has_availability` &rarr; `bool`: Indicator of whether listing is available
- `availability_30` &rarr; `int`: Number of days that the listing is available 30 days ahead
- `availability_60` &rarr; `int`: Number of days that the listing is available 60 days ahead
- `availability_90` &rarr; `int`: Number of days that the listing is available 90 days ahead
- `availability_365` &rarr; `int`: Number of days that the listing is available 365 days ahead
- `calendar_last_scraped` &rarr; `datetime`: Date since the calendar was last scraped


### Reviews Information
- `number_of_reviews` &rarr; `int`: Number of reviews of listing 

- `number_of_reviews_ltm` &rarr; `int`: Number of reviews in the last twelve months
- `number_of_reviews_l30d` &rarr; `int`: Number of reviews in the last 30 days
- `first_review` &rarr; `datetime`: Date of first review
- `last_review` &rarr;  `datetime`: Date of last review
- `review_scores_rating` &rarr; `float`: Average review score of listings across all metrics
- `review_scores_accuracy` &rarr; `float`: Average review score of accuracy
- `review_scores_cleanliness` &rarr; `float`: Average review score of cleaniness of property
- `review_scores_checkin` &rarr; `float`: Average review score of the check-in process
- `review_scores_communication` &rarr; `float`: Average review score of the host's communication
- `review_scores_location` &rarr; `float`: Average review score of the listings' location 
- `review_scores_value` &rarr; `float`: Average review score of the listings' value
- `license` &rarr; `object`: License / registration number of listings
- `instant_bookable` &rarr; `bool`: Indicator of whether the listings can be booked without host to accept the request
- `calculated_host_listing_count` &rarr; `int`: Number of active listings the host has in the current region
- `calculated_host_listings_count_entire_homes` &rarr; `int`: Number of entire homes/apt listings the host has in the current region
- `calculated_host_listings_count_private_rooms` &rarr; `int`: Number of private room listings the host has in the current region
- `calculated_host_listings_count_shared_rooms` &rarr; `int`: Number of shared room listings the host has in the current region

- `reviews_per_month` &rarr; `float`: The monthly average number of reviews over the lifetime of the listing


## Calendar Dataset Information

- `listing_id` &rarr; `int`: ID of listing

- `date` &rarr; `datetime`: Date in the listings' calendar

- `available` &rarr; `bool`: Indicator of whether the date is available for booking

- `price` &rarr; `float`: Price of listing for the day
- `adjusted_price` &rarr; `float`: The adjusted price of the listing for the day
- `minimum_nights` &rarr; `int`: Minimum nights for booking for the day
- `maximum_nights` &rarr; `int`: Maximum nights for booking for the day

## Reviews Dataset Information
- `listing_id` &rarr; `int`: ID of listing mentioned in review

- `id` &rarr; `int`: Unique ID of review
- `date` &rarr; `datetime`: Date that the review was created
- `reviewer_id` &rarr; `int`: ID of user who left the review
- `reviewer_name` &rarr; `object`: Name of user who left the review
- `comments` &rarr; `object`: Contents of review