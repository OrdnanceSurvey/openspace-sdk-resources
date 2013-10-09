OS OpenSpace SDK resources
-------

Text here..

Contents
-------

This project contains the following extensions or resources for iOS and Android SDKs.

1. OSTile offline [tile packages](#ostile-packages)
2. Offline [Places of interest gazetteers database](#places-of-interest-geocoder-database)



Resources
-------


### Offline databases

These offline databases are extensions to the both Android and iOS SDKs and can replace online access or supplement it, they can help your application overcome network coverage issues and continue to function wherever your customers are located. 

##### OSTile packages

The OSTiles format is uses the small, ubiquitous and lightweight [sqlite](http://www.sqlite.org/) database and overcomes filesystem storage problems to handle millions of images. 

OSTiles packages are sets of map tiles, each package can store several layers, a layer being a rectangular bounding box for a given Ordnance Survey product and all the map tile images to fill that bounding box. The packages are intended to transport presentational map tiles and can be used as a mechanism to allow mobile applications to display tiles offline, without the need to stream tiles from a web service.

Please refer to [OSTiles spec](ostiles_spec.md) for more details and how to create these packages.

* Demo project: [OSTileSourceDemo](https://github.com/OrdnanceSurvey/ios-sdk-demo-tilesources)


#### Places of interest geocoder database

The places of interest geocoder database is created from [OpenData](https://www.ordnancesurveyite.co.uk/oswebsite/products/os-opendata.html) products; Code-Point Open (post codes), OS Locator (Roads) and 1:50 000 scale gazetteer (place names). It is optimised for size and is packaged in the [sqlite](http://www.sqlite.org/) format as the OSTiles except with the custom file extension `.ospoi`.

Ordnance Survey will provide the tools to build this database shortly, until this is released please contact osopenspace@ordnancesurvey.co.uk if you require this feature.

* Demo project: [OSLocateMe](https://github.com/OrdnanceSurvey/ios-sdk-demo-locate-me/)