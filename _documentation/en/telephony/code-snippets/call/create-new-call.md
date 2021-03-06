---
title: Create a new call
navigation_weight: 1
---

# Create a new call

This example shows you how to make a phone call. In order to make the call, you will need to have a physical phone or softphone  

Replace the following placeholder values in the sample code:

| Key | Description |
| --- | ----------- |
| bearer_token      | Your OAuth token. [Read more about OAuth tokens](/concepts/guides/create-an-access-token) |
| account_id        | The Vonage Business Communications account ID. |
| from_destination  | NEED DOCS | 
| from_device       | NEED DOCS |
| to_destination    | NEED DOCS |
| to_device         | NEED DOCS |
| type              | NEED DOCS |

``` bash
curl --location --request POST 'https://api.vonage.com/t/vbc.prod/telephony/v3/cc/accounts/$account_id/calls' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer $bearer_token' \
--data-raw '{  
   "from": {  
     "destination": "$from_destination",  
     "type": "$from_device"  
   },  
   "to": {  
     "destination": "$to_destination",  
     "type": "$to_device"  
   },  
   "type": "$type"  
 }'
```
