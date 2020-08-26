#### From Codecademy's Data Science Learning Path

# Project Assignment: Marketing Attribution
###

CoolTShirts, an innovative apparel shop, is running a bunch of marketing campaigns to increase website visits and purchases. Using touch attribution, they’d like to map their customers’ journey: from initial visit to purchase. 

In this project, you’ll be helping them answer these questions about their campaigns:

- How many campaigns and sources does CoolTShirts use and how are they related? Be sure to explain the difference between utm_campaign and utm_source. What pages are on their website?

- What is the user journey?
  - How many first touches is each campaign responsible for?
  - How many last touches is each campaign responsible for?
  - How many visitors make a purchase?
  - How many last touches on the purchase page is each campaign responsible for?
  - What is the typical user journey?

- CoolTShirts can re-invest in 5 campaigns. Which should they pick and why?

The dataset contains one SQL table, `page_visits`. Within the table, there are 5 columns:
- `user_id` - unique identifier for each visitor to a page
- `timestamp` - time at which the visitor came to the page
- `page_name` -  title of the section of the page that was visited
- `utm_source` -  which site sent the traffic (i.e., google, newsletter, or facebook_ad)
- `utm_campaign` - the specific ad or email blast (i.e., interview-with-cool-tshirts-founder)
