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

![defaulttoken](images/defaulttoken.png "flow")

## Campaign:
###### Url Parameters - System tokens or default tokens which can be appended to the campaign URL
* {clickid}
* {campaign.id} : 81342a7e-96a9-4476-972d-21184556df1d
* {campaign.name} : Health&Nutra ENG3090G5
* {trafficsource.id} : 
* {trafficsource.name}: PropellerAds
* {device} : Mobile phone, desktop, tablet
* {brand} : samsung, Nokia, motorola, lenovo, HTC, Sony
* {model}:Samsung Galaxy S4, Opera Mini 7, Samsung Galaxy Tab 2 7.0, 
* {browser}: chrome mobile, Android Browser, Safari, Opera Mini 
* {browserversion}: Android Browser 4, Chrome Mobile 33, Chrome 31 
* {os}: Android, windows,IOS, OS X
* {osversion}: Windows 7, Android 4.1, Windows 8,
* {country}: Singapore,Cambodia, Italy
* {countryname}:
* {city}:Jakarta,Maputo,Don Bosco
* {region}: Jakarta Raya, Distrito Federal, Maputo City
* {isp}: Blackberry Limited, Telecom Italia s.p.a.
* {useragent}
* {ip}: 200.84.154.73, 103.246.201.40
* {var1}
* {var2}
* {var3}
* {var:variable name}
* {trackingdomain}
* {referrerdomain}: unknown
* {language} :Danish,Icelandic,Swahili  
* {carrier}: Blackberry Limited, Smart Axiata co. ltd.
* {connection.type} : Broadband, Mobile, Cable
* {workspace.id}
* {workspace.name}

###### Reporting Parameters
* Campaign : Health&Nutra ENG3090G5
* Campaign ID: 81342a7e-96a9-4476-972d-21184556df1d
* External campaign ID
*	Campaign URL: Unknown 
*	Campaign country tag: United States
* Campaign workspace: Private: John
*	Campaign workspace ID: 93b152bc-3f5e-4c41-b9d1-f2bc70e21eb4
*	Impressions: 1,00,000
*	Visits : 73,138
* Clicks : 16,669
*	Conversions : 676
*	Revenue  : $1,250.60
*	Cost :  $0.00
*	Profit :$1,250.60
* CPV : $0.0000
*	ICTR : 23.05%
* CTR : 22.79%
* CR : 4.06%
*	CV : 0.92%
* ROI :0.00%
*	EPV : $0.0171
*	EPC : $0.08
*	AP : $1.85
*	Errors:0
* Postback URL:	Unknown 
* Redirect: REGULAR
* Cost model: AUTO
* CPA: $0.000
*	CPC: $0.000
*	CPM: $0.000

## Offers:
###### Url Paramaters: System tokens or default tokens which can be appended to the OFFER URL
* {clickid}
* {campaign.id} : 81342a7e-96a9-4476-972d-21184556df1d
* {campaign.name}: Health&Nutra ENG3090G5
* {trafficsource.id}: 
* {trafficsource.name}:
* {lander.id}: cc6691ce-ebd0-43ae-a249-a92001627c00
* {lander.name}: Global - EN - Nutra - HTTPS
* {offer.id}: e1e72320-b46c-4fb8-b0b5-82a19395a71d
* {offer.name}: unkown
* {device} : Mobile phone, desktop, tablet
* {brand} : samsung, Nokia, motorola, lenovo, HTC, Sony
* {model}:Samsung Galaxy S4, Opera Mini 7, Samsung Galaxy Tab 2 7.0, 
* {browser}: chrome mobile, Android Browser, Safari, Opera Mini 
* {browserversion}: Android Browser 4, Chrome Mobile 33, Chrome 31 
* {os}: Android, windows,IOS, OS X
* {osversion}: Windows 7, Android 4.1, Windows 8,
* {country}: Singapore,Cambodia, Italy
* {countryname}:
* {city}:Jakarta,Maputo,Don Bosco
* {region}: Jakarta Raya, Distrito Federal, Maputo City
* {isp}: Blackberry Limited, Telecom Italia s.p.a.
* {useragent}
* {ip}: 200.84.154.73, 103.246.201.40
* {var1}
* {var2}
* {var3}
* {var:variable name}
* {trackingdomain}
* {referrerdomain}: unknown
* {language} :Danish,Icelandic,Swahili  
* {connection.type} : Broadband, Mobile, Cable
* {carrier}: Blackberry Limited, Smart Axiata co. ltd.
* {workspace.id}
* {workspace.name}

###### Reporting Parameters
*	Offer: Global - Healthy Nutrition
*	Offer ID:	e1e72320-b46c-4fb8-b0b5-82a19395a71d
* Offer URL: Unknown
* Offer country tag: Unknown
* Offer workspace : Private: Adam's Team
*	Offer workspace ID :5a280365-d9e7-4b4e-a988-051e7b0004cb
* Payout : $1.850
* Conversion cap: 
* Impressions: 0
*	Visits: 165,511
* Clicks: 23,252
*	Conversions: 2,394
*	Revenue: $4,428.90
* Cost: $1,444.13
* Profit:$2,984.77
* ICTR:0.00%
* CTR: 14.05%
* CR: 10.30%
* CV: 1.45%
* ROI: 206.68%
*	EPV:$0.0268
*	EPC: $0.19
*	AP :$1.85
*	Errors : 0


## Landers:
###### Url Parameters: System tokens or default tokens which can be appended to the LANDER URL
* {campaign.id} : 81342a7e-96a9-4476-972d-21184556df1d
* {campaign.name} : Health&Nutra ENG3090G5
* {trafficsource.id}
* {trafficsource.name}
* {lander.id}: cc6691ce-ebd0-43ae-a249-a92001627c00
* {lander.name}: Global - EN - Nutra - HTTPS
* {offer.id}: e1e72320-b46c-4fb8-b0b5-82a19395a71d
* {offer.name}: unkown
* {device} : Mobile phone, desktop, tablet
* {brand} : samsung, Nokia, motorola, lenovo, HTC, Sony
* {model}:Samsung Galaxy S4, Opera Mini 7, Samsung Galaxy Tab 2 7.0, 
* {browser}: chrome mobile, Android Browser, Safari, Opera Mini 
* {browserversion}: Android Browser 4, Chrome Mobile 33, Chrome 31 
* {os}: Android, windows,IOS, OS X
* {osversion}: Windows 7, Android 4.1, Windows 8,
* {country}: Singapore,Cambodia, Italy
* {countryname}:
* {city}:Jakarta,Maputo,Don Bosco
* {region}: Jakarta Raya, Distrito Federal, Maputo City
* {isp}: Blackberry Limited, Telecom Italia s.p.a.
* {useragent}
* {ip}: 200.84.154.73, 103.246.201.40
* {var1}
* {var2}
* {var3}
* {var:variable name}:
* {trackingdomain}:
* {referrerdomain}: unknown
* {language} :Danish,Icelandic,Swahili  
* {connection.type} : Broadband, Mobile, Cable
* {carrier}: Blackberry Limited, Smart Axiata co. ltd.
* {workspace.id}
* {workspace.name}

###### Reporting Parameters
* Lander: Global - RU - Fitness Apps - HTTPS
* Lander ID:3d29bd1b-787e-46e8-9543-749a87a8398d
* Lander country tag:Unknown
* Number of offers:1
*	Lander workspace:Private: John
*	Lander workspace ID:93b152bc-3f5e-4c41-b9d1-f2bc70e21eb4
*	Impressions:0
*	Visits: 203,125
*	Clicks:23,101
*	Conversions: 1,062
*	Revenue: $2,907.90
*	Cost:$1,250.18
* Profit: $1,657.72
*	CPV: $0.0062
*	ICTR: 0.00%
*	CTR: 11.37%
*	CR:4.60%
* CV:0.52%
* ROI: 132.60%
*	EPV: $0.0143
* EPC: $0.13
*	AP : $2.74
*	Errors: 0

## Traffic Source:
###### Reporting Parameters

*	Traffic source: Zeropark
*	Traffic source ID: 9e00c50f-3252-45cd-b134-7abc69dbea2a
*	Traffic source workspace: Public
*	Traffic source workspace ID:
*	Impressions: 0
*	Visits: 114,722
* Conversions: 2,532
* Revenue:$4,917.50
*	Cost: $0.00
* Profit: $4,917.50
*	CPV: $0.0000
* ICTR:0.00%
* CTR: 7.56%
* CR:29.20%
* CV: 2.21%
* ROI: 0.00%
*	EPV: $0.0429
*	EPC: $0.57
*	AP: $1.94
*	Errors: 0
* Postback URL: Unknown
* Click ID: Unknown
*	Cost argument: Unknown
* Variable 1
* Variable 2
* Variable 3
* Variable 4
*	Variable 5
* Variable 6
* Variable 7
*	Variable 8
*	Variable 9
*	Variable 10


## Affiliate networks:
###### Reporting Parameters

*	Affiliate network: DemoAffiliateNetwork
* Affiliate network ID: 602c0405-b98e-49ca-a0ed-2ecd61840ad0
*	Affiliate network workspace: Public
*	Affiliate network workspace ID:
*	Append click ID: No
*	Whitelisted IP:	No 
*	Impressions: 0
*	Visits:904,742
* Clicks: 59,022
*	Conversions: 13,896
* Revenue:$27,490.90
*	Cost:$3,814.94
* Profit:$23,675.96
*	CPV:$0.0042
*	ICTR:0.00%
*	CTR:6.52%
*	CR:23.54%
* CV:1.54%
*	ROI:620.61%
* EPV:$0.0304
*	EPC: $0.47
*	AP: $1.98
*	Errors: 3,276

## Traffic Source tokens

Traffic source tokens are set in TRAFFIC SOURCES FORM

![Traffic Sources Form](images/traffic.png "Traffic Sources Form")

Then in the campaign form if you select the appropriate traffic source all those tokens which are set in the traffic source form will be appended to the campaign URL

![Campaign Form](images/campaign.png "Campaign Form")

The campaign URL will look like this

http://gother-limbooks.com/81342a7e-96a9-4476-972d-21184556df1d?
zoneid={zoneid}&
device={device}&
browser={browser}&
os={os}&
country={country}&
region={region}&
isp={isp}&
useragent={useragent}&
language={language}&
connection_type={connectiontype}&
cost={cost}&
visitor_id=${SUBID}

Please note: The campaign URL can also have system tokens appended to it but all traffic source tokens are directly appended to the campaign URL only

## YouTube Video

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/KylBaHm37UQ/0.jpg)](http://www.youtube.com/watch?v=KylBaHm37UQ)
