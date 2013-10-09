OS OpenSpace SDK resources
-------

Text here..

Contents
-------

This project contains the following extensions or resources for iOS and Android SDKs.

1. OSTile offline [tile packages](#ostile-packages)
2. Offline [Places of interest gazetteer database](#places-of-interest-geocoder-database)



Resources
-------


### Offline databases

These offline databases are extensions to the both Android and iOS SDKs and can replace online access or supplement it, they can help your application overcome network coverage issues and continue to function wherever your customers are located. 

##### OSTile packages

The OSTiles format is uses the small, ubiquitous and lightweight [sqlite](http://www.sqlite.org/) database and overcomes filesystem storage problems to handle millions of images. 

OSTiles packages are sets of map tiles, each package can store several layers, a layer being a rectangular bounding box for a given Ordnance Survey product and all the map tile images to fill that bounding box. The packages are intended to transport presentational map tiles and can be used as a mechanism to allow mobile applications to display tiles offline, without the need to stream tiles from a web service.

Please refer to [OSTiles spec](ostiles_spec.md) for more details and how to create these packages.

**DEMO**

* [OSTileSourceDemo](https://github.com/OrdnanceSurvey/ios-sdk-demo-tilesources)


#### Places of interest geocoder database

The places of interest geocoder database is created from [OpenData](https://www.ordnancesurveyite.co.uk/oswebsite/products/os-opendata.html) products; Code-Point Open (post codes), OS Locator (Roads) and 1:50 000 scale gazetteer (place names). It is optimised for size and is packaged in the [sqlite](http://www.sqlite.org/) format as the OSTiles except with the custom file extension `.ospoi`.

Ordnance Survey will provide the tools to build this database shortly, until this is released please contact osopenspace@ordnancesurvey.co.uk if you require this feature.

**DEMO**

* [OSLocateMe](https://github.com/OrdnanceSurvey/ios-sdk-demo-locate-me/)


Issues
--------

For any issues relating to developing with the SDK or resources, please email osopenspace@ordnancesurvey.co.uk



Licence
-------

The OpenSpace iOS SDK and OpenSpace Android SDK are protected by © Crown copyright – Ordnance Survey 2012.[https://github.com/OrdnanceSurvey]

All rights reserved (subject to the BSD licence terms as follows):.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

- Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
- Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
- Neither the name of Ordnance Survey nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE

