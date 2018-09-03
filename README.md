/* -------------------------------- TECHNOLOGY STACK --------------------------------- */

* AWS LAMBDA
* SERVERLESS/Microservice architecture
* DYNAMO DB
* NODEJS
* I also need someone to set up an enviroment on AWS and GITHUB where multiple developers can contribute
---

/* ------------------------ LIST OF FORMS IN THE APPLICATION ----------------------------- */

* CAMPAIGNS FORM
* OFFER FORM
* LANDER FORM
* TRAFFIC SOURCES FORM
* AFFILIATE NETWORK FORM

## :green_book: LANDER FORM

When a user visits the lander URL, all the tokens are inerted to the database. The tokens can also be appended to the URL. When it is appended to the URL these tokens can be used in the landing page like shown below

Each token should be written as a seperate Lambda function.

Hello user from {CITY}  will be converted as -> Hello user from Coimbatore

![Lander Form](images/land.png "Lander Form")

Other Details that you will have to insert to the database

* Lander - Lander Name
* Lander ID - cc6691ce-ebd0-43ae-a249-a92001627c00
* Lander URL - URL of the lander
* Lander Country tag

* Visits  - The number of times the lander has be loaded in the browser
* Clicks  - The number of people who clicked the lander and visited the offer page

---

## :green_book: TRAFFIC SOURCES FORM 

There are so many traffic sources like Google, Facebook etc. Each traffic source will have its set of tokens. I will be adding all the traffic source and its set of tokens to the system.

![Traffic Sources Form](images/traffic.png "Traffic Sources Form")

---

## :green_book: Affiliate Network FORM

![Affiliate Network Form](images/affiliate.png "Affiliate Network Form")

## :green_book: OFFER FORM

![Offer Form](images/offer.png "Offer Form")

## :green_book: CAMPAIGN FORM

![Campaign Form](images/campaign.png "Campaign Form")

---

Under campaign you can link a landing page and offer page. This is a sample campaign URL

When you create a new campaign you will have to link and landing page and offer page. This URL is appended with the tokens which are provided in the traffic source form. If the traffic source is Google Adwords then the corresponding tokens are appended or if the traffic source is facebook ads then the corresponding tokens are appended.

http://gother-limbooks.com/81342a7e-96a9-4476-972d-21184556df1d?zoneid={zoneid}&device={device}&browser={browser}&os={os}&country={country}&region={region}&isp={isp}&useragent={useragent}&language={language}&connection_type={connectiontype}&cost={cost}&visitor_id=${SUBID}

When the visitor clicks the campaign he is routed to the landing page. When the user clicks the button on the landing page he is routed to the offer page.

## Flow

![Flow Form](images/flow.jpg "flow")

## System Flow
![SystemFlow Form](images/systemflow.jpg "flow")


## There are 2 kinds of tokens

![DEFAULT-TOKENS](images/DEFAULTS-TOKENS.jpg "flow")

## Campaign:
New Campaign:
{clickid}
{campaign.id}
{campaign.name}
{trafficsource.id}
{trafficsource.name}
{device}
{brand}
{model}
{browser}
{browserversion}
{os}
{osversion}
{country}
{countryname}
{city}
{region}
{isp}
{useragent}
{ip}
{var1}
{var2}
{var3}
{var:variable name}
{trackingdomain}
{referrerdomain}
{language}
{carrier}
{connection.type}
{workspace.id}
{workspace.name}
Scroll bar:
•	 Campaign
•	  Campaign ID
•	  External campaign ID
•	  Campaign URL
•	  Campaign country tag
•	  Campaign workspace
•	  Campaign workspace ID
•	  Impressions
•	  Visits
•	  Clicks
•	  Conversions
•	  Revenue
•	  Cost
•	  Profit
•	  CPV
•	  ICTR
•	  CTR
•	  CR
•	  CV
•	  ROI
•	  EPV
•	  EPC
•	  AP
•	  Errors
•	  Postback URL
•	  Redirect
•	  Cost model

•	  CPA
•	  CPC
•	  CPM

## Offers:
Available URL tokens:
{clickid}
{campaign.id}
{campaign.name}
{trafficsource.id}
{trafficsource.name}
{lander.id}
{lander.name}
{offer.id}
{offer.name}
{device}
{brand}
{model}
{browser}
{browserversion}
{os}
{osversion}
{country}
{countryname}
{city}
{region}
{isp}
{useragent}
{ip}
{var1}
{var2}
{var3}
{var:variable name}
{trackingdomain}
{referrerdomain}
{language}
{connection.type}
{carrier}
{workspace.id}
{workspace.name}
Scroll bar:
•	  Offer
•	  Offer ID
•	  Offer URL
•	  Offer country tag
•	  Offer workspace
•	  Offer workspace ID
•	  Payout
•	  Conversion cap
•	  Impressions
•	  Visits
•	  Clicks
•	  Conversions
•	  Revenue
•	  Cost
•	  Profit
•	  CPV
•	  ICTR
•	  CTR
•	  CR
•	  CV
•	  ROI
•	  EPV
•	  EPC
•	  AP
•	  Errors


## Landers:

{campaign.id}
{campaign.name}
{trafficsource.id}
{trafficsource.name}
{offer.id}
{offer.name}
{lander.id}
{lander.name}
{device}
{brand}
{model}
{browser}
{browserversion}
{os}
{osversion}
{country}
{countryname}
{city}
{region}
{isp}
{useragent}
{ip}
{var1}
{var2}
{var3}
{var:variable name}
{trackingdomain}
{referrerdomain}
{language}
{connection.type}
{carrier}
{workspace.id}
{workspace.name}
Scroll bar:
•	  Lander
•	  Lander ID
•	  Lander URL
•	  Lander country tag
•	  Number of offers
•	  Lander workspace
•	  Lander workspace ID
•	  Impressions
•	  Visits
•	  Clicks
•	  Conversions
•	  Revenue
•	  Cost
•	  Profit
•	  CPV
•	  ICTR
•	  CTR
•	  CR
•	  CV
•	  ROI
•	  EPV
•	  EPC
•	  AP
•	  Errors

## Traffic Source:

•	 Traffic source
•	  Traffic source ID
•	  Traffic source workspace
•	  Traffic source workspace ID
•	  Impressions
•	  Visits
•	  Clicks
•	  Conversions
•	  Revenue
•	  Cost
•	  Profit
•	  CPV
•	  ICTR
•	  CTR
•	  CR
•	  CV
•	  ROI
•	  EPV
•	  EPC
•	  AP
•	  Errors
•	  Postback URL
•	  Click ID
•	  Cost argument
•	  Variable 1
•	  Variable 2
•	  Variable 3
•	  Variable 4
•	  Variable 5
•	  Variable 6
•	  Variable 7
•	  Variable 8
•	  Variable 9
•	  Variable 10


## Affiliate networks:

•	Affiliate network
•	  Affiliate network ID
•	  Affiliate network workspace
•	  Affiliate network workspace ID
•	  Append click ID
•	  Whitelisted IP
•	  Impressions
•	  Visits
•	  Clicks
•	  Conversions
•	  Revenue
•	  Cost
•	  Profit
•	  CPV
•	  ICTR
•	  CTR
•	  CR
•	  CV
•	  ROI
•	  EPV
•	  EPC
•	  AP
•	  Errors



