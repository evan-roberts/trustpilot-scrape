# Python script for scraping Trustpilot reviews using Beautiful Soup

*Note that Trustpilot’s HTML may be updated, in which case you should update the `class` names in your code.*

## Update the URL

Update the `response` variable URL with your company name:

`response = requests.get(f"https://www.trustpilot.com/review/**COMPANY_NAME_HERE**?page={i}")`

## Page numbers
Update which Trustpilot pages are scraped using these variables:

`from_page = 1`

`to_page = 50`

<img width="400" alt="trustpilot_pagination" src="https://user-images.githubusercontent.com/44180246/158368492-27ca005f-92ba-4023-aedb-3f068534d7d2.png">

## Final dataframe
If you hit any Trustpilot request limits you can wait a while before running the next batch of pages.

Once you've scraped all the pages you need, you can run the last two lines to create the final dataframe `df_reviews` from the lists.

---

*You can find more details here: https://theleftjoin.com/scraping-trustpilot-reviews-with-python/*
