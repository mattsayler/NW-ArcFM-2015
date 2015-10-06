# Day 2
# Presentations

## GO165 Inspection w/Logi
### Ian Fitzgerald
### Truckee-Donner PUD

#### Logi Studio
* Build tools, web pages, dashboard widgets, maps, etc w/o code
* Pull data from about anywhere; databases, spreadsheets, services

#### Benefits
* Water usage dashboard cut down water related calls by ~75%
* Outage dashboard sometimes most used page for entire website
  * Outage map points go to device level to help obfuscate exact location
  * Research they've done, most utilities do go to house level though

* ~$13k initial purchase

---

## Confirming GPS Results
### Neal Meyer
### Central Lincoln Peoples Utility District

#### 
* Datum most likely culprit if getting high precision, but low accuracy


---

## Portal vs ArcGIS Online - When, why, and how to install each
### Skye Perry
### SSP

#### Portal
* Available w/10.3 Server License
* Tech by which most GIS data will be served up and consumed in the future

#### Utility network is Esri's new network
* In Alpha
* Non-coincident connectivity, structural associations and containment modeling
* Editing of utility network 
* Mon Oct 5th 1pm EGUG presentation

* Final release will run off of REST end points
  * Increased perf
  * Centralized Data Access
    * Avail to web maps
    * Runtime
    * 3rd Party integration
* Prepare, ~3-5 time frame

#### How to prepare
* Upgrade ArcGIS Desktop to 10.2.1
  * Will be supported until utility network is ready
* Upgrade Schneider to 10.2.1b
* Note: ONLY applies to Desktop/GDB, not to Server/Platform
* Implement a GIS Portal
  * ArcGIS Online (lower case p)
  * Portal for ArcGIS (upper case p)
  * Operational Patterns: Expose, Collect, Empower
* Begin Using ArcGIS Pro
  * Will be primary editing environ
  * BUT Pro can't edit geometric network used today
  * ArcGIS Pro is directly tied to a GIS portal
    * License admined via your portal
    * Login/data usage tied to portal
    * Runs natively off webMaps/REST Services

#### SSP's minimal recommended architecture
* Intranet
  * Esri auratative GDB
  * Internal ArcGIS Server
    * REST Endpoints
    * SSL/HTTPS
* Firewall
* Internet
  * DMZ
* CAN Store ArcGIS Server Credentials in AGOL

#### Simplified VPN model
* Use VPN instead of SSL/DMZ
* CAN'T store ArcGIS Server Credentials
* Need VPN on all internet clients

#### AGOL - Authentication
* Local Named User Strage in AGOL
  * Dedicated UN/PW
    * Must manage separate PW for these accounts
  * 
* 

#### Architecture - Portal for ArcGIS
* SSP Recommended Portal architecture
  * 
* Fully Secured via ssl
* All Authentication components behind the firewall
* Full Portal access via the internet
* All Authorized devices can access via internet
* Full editing available
* 

#### 3 Approaches to using Portal
1 _Register REST Services_ Manually
  * 
  * Publish MXD to REST Service
  * Loosely coupled
2 _Federating_ ArcGIS Server via Portal
  * Switch your ArcGIS Server authentication to utilize Portal
  * When users publish MXDs to Server, Automatical Creation of Service Items in Portal
    * Keeps items in sync between Server and Portal
  * Sever and Portal MUST be same release
3 Designating Portal as a _Hosted Server_
  * Similar to Fed. but Portal now has a dedicated GDB
  * Publishers/admins in Portal can add hosted feature services

* Note: can have _multiple_ federated servers with Portal but only _one_ hosted server

####
* Portal provides siginfigant value at significant cost
  * Pros
    * On premise
    * Easier integration with AD
    * Federation is nice to have
    * Allows you to own the entire solution
  * Cons
    * Additional hardware
    * Additional project cost
    * Higher support cost

* AGOL
  * Pros
    * Full SAAS
    * data maintained on premise
    * Esri handles quarterly releases, support, etx
    * Lower cost of ownership
  * Cons
    * Challenging integration with AD
    * 

* Largely comes down to Authentication & money
* All things being equal, SSP recommends ArcGIS Online whenever possible due to better benefits and a lower total cost of ownership

www.slideshare.net/sspinnovations

---

## Douglas County PUD Upgrade to 10.2.1
### Kevin Vaughn
### Douglas County PUD

#### Stack
* ArcGIS 10.2.1
  * ArcMap
  * ArcGIS Engine
* ArcFM 10.2.1a
  * ArcFM
  * Fiber
  * Designer
  * Viewer
* SSP
  * WFM
  * Transformer manager
  * Pole manager
  * Hyperlink manager
  * Unitization
  * UG cable tagging
* DCPUD
  * Search tool
  * Location info

#### Unexpected Functionality
* Discovering old mistakes
* Trouble with DCPUD search tool
* SE Bug MM54635
  * Has to do w/adding related units
  * Unsure if SE bugs fixed in b
* SE Bug MM55143
  * Sometimes Update button in ArcFM Attribute Editor doesn't activate
  * Think is fixed in b
* FM2.0 & Labeling in the Viewer

#### Overall
* Went pretty well, minimal issues
* Upgrade ~3 month process
* 

#### Things they like
* Find feeder tool
* About 2 seconds to trace feeder
* Editing faster
* FM2.0 Fields
* 

---

## Automating Feeder Maps Using Data Driven Pages and Arcpy
### Matt Sayler
### Clark Public Utilities

#### https;//mattsayler.github.io/Automating_Feeder_Maps_Presentation/

---

## Birds of a Feather

#### Issues
* Multiple Utilities: Data view/refresh/scroll bars disappear
  * Still issue
  * Send to Keith, verify it's documented
* Multiple utilities: Page dimensions coming in at null dimensions, so no map in layout view until update page or pick saved layout
* Chelan PUD: ArcMap, switching between multiple page sizes, sometimes can't print. Have to go back to data view then pick layout
  * possibly fixed in 10.2.1a
* ArcFM Attribute Editor, Silicon Valley: Error when selecting multiple features (Shift-click, ctrl_click) & remove from selection. Second attempt at same process works.
* Pend Orielle PUD: Pictometry tool bar crashes edit sessions sometimes
* Pend Orielle PUD: Issues with FM2.0 and selections/spatial queries
* Cowlitz and PGE: "Object refernce not set to instance of an object" sometimes when editing network features.
* Cowlitz: Issue replacing service with python script
* 
