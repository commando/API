CHANGELOG
=========

## v1 - 7/9/2015

- Added the get all in the execution queue endpoint `/execution-queue`.

## v1 - 7/8/2015

- Added recipe argument support in `/recipes/:id/execute`. You may now optionally pass a JSON string object in the post parameter `recipe_arguments`. See the following curl example:

````
curl -u foo:skey_2azljcEZBjjxKQ53cf5cc807a673EqqdNmT https://api.commando.io/v1/recipes/rec_3Fc5q540e480b672d38Ig/execute -X POST -d "groups=grp_2Xk7x540e481bcb9c775d" -d 'recipe_arguments={"$host":"google.com"}'
````

## v1 - 3/12/2015

- Changed how servers are returned in endpoints `/groups` and `/groups/:id`. They now return an array of objects.

````
"servers": [
    {
    	"id": "srv_9GkE2IWvkzItmaTs5Agn8",
    	"label": "WEB1"
    },
    {
    	"id": "srv_5EdvDbyOtmF9nXS7ZowcB",
    	"label": "WEB2"
    }
]
````

Previously:
 
 ````
"servers": [
    "WEB1",
    "WEB2"
],
"servers_ids": [
    "srv_9GkE2IWvkzItmaTs5Agn8",
    "srv_5EdvDbyOtmF9nXS7ZowcB"
]
 ````
 
## v1 - 11/17/2014

- Added the following endpoints: `/servers`, `/servers/:id`, `/groups`, `/groups/:id`, `/recipes`, `/recipes/:id`

## v1 - 9/23/2014

- Initial release.
