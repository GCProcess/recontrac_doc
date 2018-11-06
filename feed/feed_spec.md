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
The FTP destination for file feeds is: ​ ftp.recon-trac.com

The username and password will be provided as needed.

The typical feed has the following fields (Bold are required, missing items should be blank but not excluded, the more the better):

**Ord**|**Name**|**Example**|**Ord**|**Name**|**Example**
:-----:|:-----:|:-----:|:-----:|:-----:|:-----:
 | | | | | 
1|UsedNew |NEW/USED/N/Y |23|AutoID | 
 | | | | | 
2|Year |2013|24|InternetSpecial | 
 | | | | | 
3|Make |Honda |25|InventoryDate |5/23/13 21:49
 | | | | | 
4|Model |Civic Cpe |26|CarfaxOneOwner | 
 | | | | | 
5|Trim |Si |27|CarfaxAvailable | 
 | | | | | 
6|BodyStyle |2dr Man Si |28|VideoPlayerUrl | 
 | | | | | 
7|StockNumber |DH703792 |29|VideoEmbedUrl | 
 | | | | | 
8|VIN |2HGFG4A58DH703792 |30|LastUpdated |5/23/13 21:49
 | | | | | 
9|Mileage |9|31|Custom1 | 
 | | | | | 
10|Price | |32|Custom2 | 
 | | | | | 
11|Engine |2.4L 4 Cylinder Engine |33|Custom3 | 
 | | | | | 
12|Tramsission |6-Speed M/T |34|Custom4 | 
 | | | | | 
13|Color (External) |Dyno Blue Pearl |35|Custom5 | 
 | | | | | 
14|Interior (Color) |Black |36|LastPhotoUpdateUtc | 
 | | | | | 
15|Comment | |37|Doors |2
 | | | | | 
16|Options | |38|ModelSeries | 
 | | | | | 
17|LotPrice | |39|EngineCylinders |4
 | | | | | 
18|MSRP |23305|40|MPG\_City | 
 | | | | | 
19|Invoice | |41|MPG\_Highway | 
 | | | | | 
20|ImageURLs | |42|Fuel\_Type | 
 | | | | | 
21|Certified |MANUFACTUR |43|Cab\_Type | 
 | | | | | 
22|ModelCode |FG4A5DJW |44|Cost | 
 | | | | | 