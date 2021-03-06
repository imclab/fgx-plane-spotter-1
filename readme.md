FGx Plane Spotter Read Me
=========================

<iframe src=http://jaanga.github.io/fgx-plane-spotter/latest/index.html width=96% height=600px >
Visible only in HTML view here: http://jaanga.github.io/terrain-viewer/fgx-plane-spotter/ </iframe>  
_Cropped iframe view of FGx Plane Spotter latest revision_

Live demo: [FGx Plane Spotter (latest)]( http://jaanga.github.io/fgx-plane-spotter/latest/index.html "Happy spotting!")  
	
- Latest: r3
- Loads and displays all ICAO, navigation aids, helicopter pad and seaplane ports. See Help for color code
- Bugs fixed that slowed things

Live demo: [FGx Plane Spotter r1]( http://jaanga.github.io/fgx-plane-spotter/r1/index.html "Happy spotting!")

* Earlier revision with some features not in the current release

For the generic 3D map used as the basis here see also: [ Jaanga Terrain]( http://jaanga.github.io/terrain/ )  
For other viewers of the data see also: [Jaanga Terrain Viewer]( http://jaanga.github.io/terrain-viewer/ )

For [Leap Motion]( http://www.leapmotion.com/ ) device enabled and earlier versions see: [Flying Leap 3D]( https://github.com/jaanga/gestification/tree/gh-pages/projects/flying-leap-3d )

## Concept
View live [FGx Crossfeed]( http://crossfeed.fgx.ch/data ) data - showing current FlightGear sessions - in the context of an interactive 3D map with 18 levels of zoom.

## Features
* Shows FGx Crossfeed aircraft in 3D
* Displays much data including ILS cones for 2,136 airports and some data for over 27K ICAO listings 
* Places dropdown lists the airports. 
* See also the features of [Jaanga unFlatland]( http://jaanga.github.io/terrain-viewer/un-flatland/ ).
	- FGx Plane Spotter is an app built on top of unFlatland which is a viewer of 3D [Jaanga Terrain]( http://jaanga.github.io/terrain/ ) data.

## Road Map

### Overview
The current app shows an amusing, hopefully, toy-like view of the FGx Crossfeed data.
There is, however, nothing stopping FGx Plane Spotter from becoming an extremely serious and useful on-line mapping and tracking app 
- useful for FGx Crossfeed data and for any application that wants to display movements of a global nature.

The wish list of possibilities has been started - and many more items can be added

But, before that work proceeds in earnest on the specific item wish list, there are three significant repositories that need to be updated or created and in operation.

Each of the three is an amusing, challenging job in its own right. No task is particularly difficult. 
The challenge is finding cool ways of automating the processes and procedures.


### 1. FGx Terrain
The proposed work is described in detail here: 

* [Fgx Terrain]( https://github.com/fgx/fgx-terrain/ )  
* [Jaanga Terrain Read Me]( http://jaanga.github.io/terrain/index.html ).

The FGx crew should decide whether or not FGx wishes to take on the terrain elevation bitmap project and create and maintain the repository and its data.

### 2. FGx Aircraft
The proposed work is described in detail here: [FGx Aircraft]( http://fgx.github.io/fgx-aircraft/index.html#roadMap )

The FGx crew should decide whether or not FGx wishes to take on the aircraft repository (and browser/viewers) projects and create and maintain the repositories and their data.

### 3. FGx Airports
The current location used by FGx Plane Spotter to access ICAO airport, runway and navaid data is via linking to a sub-directory in a repository belonging to Geoff here:

<https://github.com/geoffmcl/map-test2/tree/gh-pages/data>

The FGx crew should decide whether or not to bring in Geoff's and maintain it as a standalone repository that can be used by a variety of apps built by FGx or by others.


### Repository Tiles
The titles of the above-mentioned three repositories are suggestions only.
But the idea should be that a first time visitor to the FGx site has a fairly clear picture of what they are likely to find in a repository._



## Issues /Bugs

* <s>Jerky 'myplane' with incorrect heading</s>

## Project Links

Given the current CORS issues, you now have four ways of viewing the FGx Plane Spotter files:

* Code hosted on GitHub: [jaanga.github.io]( http://jaanga.github.io/fgx-plane-spotter/ "view the files as apps." ) <input value="<< You are now probably here." size=28 style="font:bold 12pt monospace;border-width:0;" >  
* Source code on GitHub: [github.com/jaanga]( https://github.com/jaanga/fgx-plane-spotter/ "View the files as source code." ) <scan style=display:none ><< You are now probably here.</scan>

or 

* Code hosted on GitHub: [fgx.github.io]( http://fgx.github.io/fgx-plane-spotter/ "view the files as apps." )    
* Source code on GitHub: [github.com/fgx]( https://github.com/fgx/fgx-plane-spotter/ "View the files as source code." )  

FGx home page: [fgx.ch]( http://www.fgx.ch )

For a reference as to the name of this repository see also [Aircraft Spotting]( http://en.wikipedia.org/wiki/Aircraft_spotting )



## Copyright Notice and License

[FGx copyright notice and license]( https://github.com/fgx/fgx.github.io/blob/master/fgx-copyright-notice-and-license.md )

This app is at an early and volatile stage. Not all licensing requirements may have been fully met let alone identified. It is the intension of the authors to play fair and all such requirements will either be met or the feature in question will turned off.


## Change Log

2014-03-16 ~ Theo

* Code clean up
& Fix Cmera to ATC

2014-03-12 ~ Theo

* r3 committed

2014-02-20 ~ Theo

* Stingier hashes and permalinks
* Started Adding camera position and target permalinks
* Continued code cleanup now that no longer need to read two icao files.
* Updates to menu and read me files

2014-02-18 ~ Theo

* Fixed Geoff's 'iles' find
* Just reading apt1000-icao and the extractinf icaoGazetteer and ilsGazetteer from that.
* Undid previous because 200 JSON files do not exist
* Exclude anything not pure ILS from ILS
* Load and draw all icao, heli, nav and sea
* Redo the 'Just reading...' because I found I was loading the wong file
* Add onerror to loading heitmaps
* add 'latest' folder and index
 


2014-02-15 ~ Theo

* Comments added to code. Minor code clean-up
* Reset camera position and target with each change of location
* Add change camera target to ATC
* Some playing with colors, shapes and sizes
* Tiny bit of mouseover action

2014-02-14 ~ Theo

* Cleaned up the menu structure
* More robust permalink system - orderless, sparse and selective
* Fixed the ILS pointing under ground thing. It was a degree to radians thing

2014-02-13 ~ Theo

* r2.4
* Fixed broken permalink maker
* Added clear permalink button

2014-02-12 ~ Theo

* r2.3
* Added rev number variable
* Status div now movable and resesizable;

2014-02-11 ~ Theo

* r2.2
* There are aircraft in the air. Many issues.

* r2.1
* ILS points in correct direction, angle adjusted
* only show ils.type = ils
* Correct length of ILS cone displaye
* Areas not in 3D have reduced opacity, text message dsplayed
* Permalinks start to work
* Many of the navaids in

2014-02-10 ~ Theo

* r2 committed ~ 90 meter resoution. ILS and runways for 2136 airports
* In the jaanga project until CORS/forking strategy is worked out
* Many read me file updates
* Length of ILS beam may now be correct

2013-12-20 ~ Theo

* Aicraft no longer jiggles, visible with all cameras
* Support for canvas renderer added

2013-12-17 ~ Theo

* Update read me


2013-12-16 ~ Theo

* Added ability to load an aircraft and tie it to camera position

2013-12-15 ~ Theo

* R1 added. Fork of unFlatland R4
* Changed places to listing of airports with ILS
* Added tooltips to places dropdown
* Added listening to FGx Crossfeed and displaying 'Seymour' in appropriate location with heading


