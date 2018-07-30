## :boom: Introduction

This is how a typical URL looks

http://gother-limbooks.com/81342a7e-96a9-4476-972d-21184556df1d?zoneid={zoneid}&device={device}&browser={browser}&os={os}&country={country}&region={region}&isp={isp}&useragent={useragent}&language={language}&connection_type={connectiontype}&cost={cost}&visitor_id=${SUBID}

If you refer the above, certain query string are provided by the traffic source and certain will have to be provided by us. For example in the case of ad network propeller ads, the below are the ones provided by them

```
zoneid={zoneid} - Zone id is the placement id where our ad is shown
```

In future these ad works might start providing more tracking tokens

Now in the above URL these are the ones which we will have to populate and not provided by propellerads. These are the default query string that our software should provide

```
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
{var1} -
{var2}
{var3}
{referrerdomain} 
{language} - browser language
{connection.type}  - broadband or wifi or carrier
{carrier} - Airtel or Vodafone or Jio etc
```

If the adnetwork provides city and state tokens, it is not necessary that I use our tokens rather I can use the adwetworks tokens.

---

## :boom: Tab - Landers: 

Landing page is basically a presales page

Under this menu I would be able to create any number of landing pages

Fields:

* Lander Name: 
* Lander URL: 
  
---

## :boom: Tab - Offers: 

Usually companies outsource their marketing needs to a third party. These third parties create a new landing page on top of the offer page.

 Offer is the real landing page of the company


Fields:

* Offer name: 
* Offer URL: http://in.crigroups.com/index.html?cid={clickid}

---

## :boom: Tab: campaign: 

 * Campaign name: 
 * Country: Drop down:
 * Traffic Source: 
 * Landers: Drop down - Select the lander which you have already created
 * Offers: Dropdown - Select the offer which you have already created

  Here you are linking both the lander and offer. Campaign tab will provide you a new URL. This is the URL which you use in traffic sources like google adwords, bing, trafficvance etc.

---

## :boom: Tab: Traffic sources

 * Traffic Source name: 


---


