#test api call
import requests
import json
import pycurl
import ast

api_token= "<TOKEN>"
api_url_base = "https://freefeed.net/v2/users/whoami"
headers = {'x-authentication-token':api_token}


response = requests.get(api_url_base,headers=headers)

content= response.json()
print(type(content))

d=json.dumps(content,indent=12)
print (type(d))
#print(d)



for i in content['users']:
    print(i)
    for k,v in i.items():
        if k == 'username':
            print(v)
