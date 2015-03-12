CHANGELOG
=========

## v1 - 3/12/2015

- Changed how servers are returned in endpoints `/groups` and `/groups/:id`. They now return an array of objects.

````
"servers": [
    {
        "id": "srv_GyrjA546fe7e6cc2fauny",
        "label": "BENCH2"
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

## v1 - 9/23/2014

- Initial release.
 
## v1 - 11/17/2014

- Added the following endpoints: `/servers`, `/servers/:id`, `/groups`, `/groups/:id`, `/recipes`, `/recipes/:id`
