# ReconTRAC Default File Specification

    Green Cloud Process, Inc.
    ReconTRAC
    Dealer Integration

At no extra cost, ​ReconTRAC​ can receive daily inventory feeds from the dealer to help employees create jobs more efficiently by pre-filling data based on a stock number or part of a VIN.

Often these feeds are provided by third-party providers like vAuto or in some cases, internal IT departments. This is the exact same feed that the dealer sends to web sites such as http://www.cars.com​ and ​www.autotrader.com​.

This is public information found on the web and contains no proprietary data.
Typically, the process for setting up the feed is a three step process:

## Steps
* The Dealer needs to inform its Inventory Feed provider of the need to send their feed to a new feed recipient (Green Cloud) and inform Green Cloud of contact information for VIN provider.
* Green Cloud contacts the VIN feed provider and sets up VIN feeds to the Green Cloud servers.
* Once feed is received from VIN feed provider, the data is validated and imported into the system. Once it’s set up, it’s automatic every night.

## Technical Details

Feeds are provided typically as a file (Comma delimited/​CSV​) that is sent to Green Cloud electronically through FTP (File Transfer Protocol). They can follow a few formats but typically they would follow the same format that is sent to internet companies like​ cars.com.

Each dealer typically uses a custom username/password to pass this file to Green Cloud/ReconTRAC but in some cases dealer groups have passed one large file with multiple dealers vehicles.

### FTP Details
* The FTP destination for file feeds is: ​ **ftp.recon-trac.com**
* The username and password will be provided as needed.

The typical feed has the following fields (Bold are required, missing items should be blank but not excluded, the more the better):

**Ord**|**Name**|**Example**|**Description**|
:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
1|UsedNew |NEW/USED/N/Y | Whether user or new |
2|Year |2013|Vehicle year |
3|Make |Honda | Vehicle Make |
4|Model |Civic Cpe | Vehicle Model |
5|Trim |Si | Trim Type |
6|BodyStyle |2dr Man Si | Body Style |
7|StockNumber |DH703792 | Stock Number |
8|VIN |2HGFG4A58DH703792 | VIN Number |
9|Mileage |9| Mileage |
10|Price | 23400.00 | Listed Price |
11|Engine |2.4L 4 Cylinder Engine | Engine Type |
12|Tramsission |6-Speed M/T | Transmission |
13|Color (External) |Dyno Blue Pearl | External color |
14|Interior (Color) |Black | Interior color |
15|Comment | | Any vehicle comments |
16|Options | | Vehicle Options |
17|LotPrice | 35500.00 | Price on lot |
18|MSRP |38600.00| MSRP Price |
19|Invoice | 12345A | Invoice number |
20|ImageURLs | | URLs of images |
21|Certified |MANUFACTUR | Who certifies vehicle |
22|ModelCode |FG4A5DJW | Manufacture model code |
 23|AutoID | A1234 |Auto Identifier  |
 24|InternetSpecial | T| Id vehicle internet special |
 25|InventoryDate |5/23/13 21:49 | Date vehicle entered inventory |
 26|CarfaxOneOwner | T | Carfax shows one owner |
 27|CarfaxAvailable | T | Whether carfax is available |
 28|VideoPlayerUrl | | Video Player URL |
 29|VideoEmbedUrl | | Video URL |
 30|LastUpdated |5/23/13 21:49 | Last time vehicle was updated |
 31|Custom1 | | Custom field 1 |
 32|Custom2 | | Custom field 2 |
 33|Custom3 | | Custom field 3 |
 34|Custom4 | | Custom field 4 |
 35|Custom5 | | Custom field 5 |
 36|LastPhotoUpdateUtc | 5/23/13 21:49 | Last time photo updated in UTC |
 37|Doors |2 | Vehicle Doors |
 38|ModelSeries | A | Model Series |
 39|EngineCylinders |4 | Engine Cylinders |
 40|MPG\_City | 24 | MPG in City |
 41|MPG\_Highway | 33 | MPG on Highway |
 42|Fuel\_Type | Unleaded | Type of fuel |
 43|Cab\_Type | Sedan | Type of CAB style |
 44|Cost | 33541.00 | Aquire Cost |
 | | | |
