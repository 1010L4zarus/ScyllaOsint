# ScyllaOsint

# Scylla - The Simplistic Information Gathering Engine
<p align="center">
  <img src="https://github.com/josh0xA/Scylla/blob/master/imgs/Screen%20Shot%202020-05-10%20at%206.43.35%20AM.png?raw=true">
</p>



## Installation
1: ```git clone https://github.com/MandConsultingGroup/Scylla```<br/>
2: ```cd Scylla```<br/>
3: ```pip install -r requirments.txt```<br/>
4: ```scylla.py --help```<br/>


## Menu
```
usage: scylla.py [-h] [-v] [-ig INSTAGRAM] [-tw TWITTER] [-u USERNAME]
                 [--info INFO] [-r REVERSE_PHONE_LOOKUP] [-l LOOKUP]
                 [-s SHODAN_QUERY] [-g GEO] [-c CARD_INFO]

optional arguments:
  
  -h, --help            show this help message and exit
  
  -v, --version         returns scyla's version
  
  -ig INSTAGRAM, --instagram INSTAGRAM
                        return the information associated with specified
                        instagram account
  
  -tw TWITTER, --twitter TWITTER
                        return the information associated with specified
                        twitter account
  
  -u USERNAME, --username USERNAME
                        find social media profiles (main platforms) associated
                        with given username
 
 --info INFO           return information about the specified website(WHOIS)
                        w/ geolocation
 
 -r REVERSE_PHONE_LOOKUP, --reverse_phone_lookup REVERSE_PHONE_LOOKUP
                        return information about the specified phone number
                        (reverse lookup)
  
  -l LOOKUP, --lookup LOOKUP
                        performs a google search of the 35 top items for the
                        argument given
  
  -s SHODAN_QUERY, --shodan_query SHODAN_QUERY
                        performs a an in-depth shodan search on any simple
                        query (i.e, 'webcamxp', 'voip', 'printer', 'apache')
 
 -g GEO, --geo GEO     geolocates a given IP address. provides: longitude,
                        latitude, city, country, zipcode, district, etc.
  
  -c CARD_INFO, --card_info CARD_INFO

```
## API NOTICE
The API used for the reverse phone number lookup (free package) has maximum 250 requests. The one used in the program right now will most definetely run out of uses in the near future. If you want to keep generating API keys, go to https://www.numverify.com, and select the free plan after creating an account. Then simply go scylla.py and replace the original API key with your new API key found in your account dashboard. Insert your new key into the keys[] array (at the top of the source). For the Shodan API key, it is just a sample key given to the program. The developer recommends creating a shodan account and adding your own API key to the shodan_api[] array at the top of the source (scylla.py). 
