# Day 1

## Schneider Update
### Matt Zimmerman

#### Misc
* Schneider partnered with Geocortex
* ArcGIS Portal Certified - can install, configure etc
#### Technology Update
* 10.2.1b
  * FM 2.0
    * Support for customizations
    * Improved performance
    * Improves editing patterns
      * Moved sync'ing to backend (if you want)
      * Backend tool to sync FeederIDs
      * Customizations driven by change in FeederID field not supported
      * APIs for sync
      * Button for sync
    * Customer highlight: APS
      * One session, 32 steps
      * From 42 min to 4 min
      * Note this is NOT a Schneider test
    * Trial Program
      * Temporarily turn on FM 2.0 to test out
  * ArcFM Solution
      * Sort and group CUs
      * New Commissioning patterns (Designer Express)
      * High res printing in Silverlight (FINAL enhancements)
  * Responder
      * More restoration workflows - jumpers and phase swap
      * New user requests - 24+
      * Weather web services - Real-time
        * Rated most accurate
        * 60 day trial
  * Fiber Manager
      * Better ID tool
      * Reduced training time
      * Supports initial cust location info
  * Tech Support
      * Updateable installer - simple update to go to 10.2.1b (like patch)
      * Oracle 12c
      * ArcGIS Server 10.3.1 - fully supported by 10.2.1b
      * Only desktop & SDE need to be 10.2.1
  * Best Practices White Papers
      * Find on Exchange
* ArcFM Mobile - (Rebranded/Repackaged Orbit)
  * Field Work
    * Current work
    * Navigation
    * Collect and distribute data
    * New at 2.1: Offline, Redlines
    * REST services, can sync with Asset Management, etc w/o going through GIS
  * Viewing
    * Offline access
    * ArcFM tools in field (tracing still on the way)
    * View & Query
    * Can swap viewer licenses for mobile licenses (lower cost too)
  * (Mobile not for editing the data yet, different usage pattern)
* Looking Ahead: Winter Agenda
  * ArcFM Essentials
    * HTML5-based Viewer
      * ArcFm tools & workflows
      * Get ansers via viewing analysis and network interrogation
      * Mobile & desktop
      * Reduce need for custom code
      * Get more out of the portal and named users
    * Next steps
      * Parity w/Silverlight
        * Swap program
      * Add additional util workflows
      * Build on mobile tech
  * Responder 
    * Thin Client
      * Easy/fast deployment
      * Integrating with Geocortex?
        * Maybe? Dev started prior to partnership.
    * New mobile app
      * Collect outage info
    * Product adapters
      * Prepackaged for IVR, AMI, etc
  * ArcFM Mobile for iOS
    * Round out field inspection and maintenance workflows
      * Xfmr & assembly inspections
        * Q: How configurable are inspections? A: Very
      * Network interrogation
      * Admininster daily work to crews
    * Q: Mobile for Android? A: Will start to merge stuff in HTML5 solutions (trying to move to platform agnostic solutions)
    * Q: Inspections pushed to place where can be approved? A: Yes
  * Offline Data Manage
    * New solution to manage and sync large data sets
      * Via Esri's latest sync tech
      * Scalable
        * After ~500,000 records, gigs of data
      * UX for tier one utility requirements around multi-region
        * Ability to regionalize data
      * For mobile, web, & desktop
      * Centralized administration
      * Est. November release
  * Smart Network Design
    * Working on next gen design product
    * Note this is long term, 3-5 year project
    * Simple & Powerful
    * Efficient design
      * Support working disconnected
        * Support contractors
    * Lower cost of ownership for GWD
      * One tool
      * Design wherever
      * Just works
      * For engineers (who shouldn't need to be GIS Experts)
      * Toolset for ArcGIS Pro for GIS people (see below)
    * Reduced backlog
    * Improved reliability
    * Strategy
      * Electric and telecom first
      * Workflow focused releases
      * Use of ArcGIS Pro for commissioning
    * Engineering Network Model
      * A new network backbone for advanced network management tools
      * _Adds_ to model
      * Release ~Winter 2016
      * Network interrogation
      * Engineering analysis
        * Leverage Schneider's vast DMS knowledge
      * Design optimization
    * Evolving w/Esri
      * Smart Network design - Esri SDK
      * Designer HFC - 
      * ArcFM components - 
      * Data replication - 
      * Get familiar with Esri named users, may become Schneider requirement for next gen tech
        * Group Comments: 
          * Want ability for windows credentials to pass through, no secondary sign-on
            * Keith checking on this
          * Adds additional account management overhead

---

## ArcFM Essentials: The What the Whys and the Hows
### Frank Towler
### Latitude Geographics

#### Why
* One point of contact, one license agreement
* Bundled Support
* Esxisting ArcFm server users will not need to purchase ArcFM Essentials
* Facilitates move to HTML5
* Mutual clients get a "best of breed" solution
* Enable smore innovation for utility solutions
#### How Does this impact my company?
* ArcFM Essentials = Geocortex Essentials + Utility Enhancements
#### Who are we?
* Esri Platinum Partner
* Victoria, BC
* 100+ staff
* 1000+ clients worldwide
* 25% buisiness through resellers
* Debt free, profitable & owner operated
#### Technology for Consumers
* Map viewers for all major platforms
* Toolset for end users, no coding
* Mobile
  * Support disconnected
* Intuitive, Guided Interactions
* Have customers that buy it JUST for 
  * Reporting
  * Printing
* Instant Search
* Dynamic Charting
* Datalinking
  * Connect to non-spatial data from Oracle or SQL Server & maintain data where it belongs
* Security
#### Technology for Producers
* Avoid one-offs and pointed solutions by re-using common building blocks for all your apps
* Workflow Technology
  * Easily build simple guided Activities
  * Huge library of pre-built Activities
  * Drag and drop tool building
  * 99% of time workflow can be built using existing Activities
  * Can consume Model Builder tools
* Rich Developer SDKs
#### How can I get ArcFM Essentials?
* Through ELA
* If you have ArcFM Server, can get free
#### Group Questions
* Secure login available? A: Yes
* Down to field level, like User A can see fields User B can't? A: yes

---

## 
### Keith Krall
### Esri

* Esri Videos: E380

#### 10.2.1
* 700+ fixes
* Released Jan 2014

#### 10.1 SP1 QIP & 9.3.1 QIP
* 400+ fixes
* March 2014

#### Consumerization of IT
* Peoples expectations
  * Smart devices
  * Do the things they're able to do at home at work
  * BYO Device

#### Core ArcGIS Online Configuration
* ~3 days

#### Web GIS Includes Online Analytic Services

#### HERE Maps
* HERE, Formerly Navtech
* Collect LIDAR with street level imagery
* Can measure features in webmap

#### solutions.arcgis.com
* Templates for web apps
* Try It Now for demo site

#### ArcGIS Pro
* Desktop not moving to 64bit, Pro is the 64bit direction

---

## Panel Discussion

* Inspector/Redlining: What is going to happen with classic Inspector product?
  * Matt Z: On 10.2.1, but probably no further development, on 6 year support cycle. Swap program with ArcFM Mobile.
  * Pacificorp: Replacement really needs to support multi-level and one-to-many relationships
* Will the session manager user experience be improving? Clunky, 
  * Not likely. Older technology. 
* 

## Business Meeting
* Elections 
  * President: Kevin Vaughn - Douglas County PUD
  * Vice President: Wendy Largent - Umatilla PUD
  * Secretary: TBD
* Host for 2016
  * Keeping Tues/Wed (~13th/14th Sept 2016)
  * TBD: Esri Olympia? Clark? NW Natural?
