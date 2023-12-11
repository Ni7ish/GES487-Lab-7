Nitish K Singh
Graduate Project Tutorial

Lab 7 – Leaflet Side-By-Side Map

Goal: The purpose of this tutorial is to create a basic webpage that displays a single panel with two maps displayed side-by-side with manipulable controls that translate any swipes to movement over both maps simultaneously.
The displayed maps are overlayed over each other so that the central divider allows a comparison of two maps over a singular viewing range.

Step 1: Access this link on GitHub and download the fileset as a zip file to your computer. Click the green <>Code button for a dropdown menu to the download.
 
Step 2: Extract downloaded files to a location of your choice.
Step 3: Open file ‘index.html’ in a word editing program, preferably NotePad++ (Used here)
 

Step 4: The first edit needed to be made to the file in order to ensure up-to-date functionality is to change the Leaflet version calls within line 7 and 9. This ensures the latest version of Leaflet is being accessed by the file.
To find out which version of Leaflet is current, search for or access the download page via this link. The first version displayed in the ‘Download Leaflet’ category is the currently hosted version as follows:
 
Change highlighted and redlined version numbers in the ‘index.html’ file:
 
Step 5: Find out coordinates for initial loading point of the map, whether from a pre-existing source or as desired. Steps to find one on your own:
Visit maps.google.com in a browser and navigate to the desired location:
 
Step 6: In the address bar of the browser, locate the Decimal Degrees coordinates for the current area of view.
 
Coordinates: 61.3765647,5.6314515
Step 7: Copy or make note of numbers in any location or edit the ‘index.html’ file in the body, as follows:
 
NOTE: Fewer decimal places are possible to use but may result in slight deviation of map center from original location. Number subsequent to the Decimal Degrees value is the current Zoom level value the map initially loads in at. It may require to be changed if the selected basemap has limitations in Zoom range.
Step 8: Locate Basemap for use at Leaflet using this link.
Locate desired Basemap and copy variable text with embedded link titled : Plain Javascript
 
 
Replace variable text in ‘index.html’ with copied version and repeat as necessary for both map variables.
 
 
Changed to:
 
NOTE: Both variables MUST include ‘.addTo(map)’ function at the end of variable creation, since both maps must appear simultaneously.
Step 9: Once variables for both maps are created/edited, the function for the side-by-side map should be called/edited using recently updated variable names as follows:
 
This will ensure the appropriate basemaps are used when the webpage and map load.
Experiment as desired to incorporate into other map pages you may have created.
 
Final Output:
 
Note: On certain (most) browsers, the center controller does not work and the map must be navigated using regular left-click and drag mouse functions.


END



References
Base Files: digidem/leaflet-side-by-side: A Leaflet control to add a split screen to compare two map overlays (github.com)
Editor: Downloads | Notepad++ (notepad-plus-plus.org)
Leaflet version: Download - Leaflet - a JavaScript library for interactive maps (leafletjs.com)
Leaflet Basemaps: Leaflet Provider Demo (leaflet-extras.github.io)
Maps Coordinates: Google Maps
