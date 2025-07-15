
# agol-autocad-interface
Accessing layers from AGOL using AutoCAD plugins to avoid double-handling datasets.
---

## Installation and running the plugin
The latest release can be found in [Releases](https://github.com/GWP-Consultants/agol-autocad-interface/releases)

Download this .zip file onto your computer and unzip.

Open AutoCAD and run:

        netload
Then navigate to the directory where the plugin was unzipped and select 

		ArcGISAutoCAD.dll
The plugin will be initialised and ready to use from the ribbon at the top.
First use the 'Settings' button to log in to your AGOL account and select the destination CRS you intend to use.
Next the import button will display available folders to the logged in user and their subsequent layers.
Multiple can be selected at once to allow for easier loading.
If a point layer is chosen the user is prompted to choose whether this should be loaded as a default circle or inherit a block reference.
A number of default block references are also used by the plugin.
If the block reference has an attribute defined then the plugin will prompt the user to choose an attribute from the AGOL layer to fill this for each item within the layer.

---

## Access as of July 2025  
The latest release can be found in [Releases](https://github.com/GWP-Consultants/agol-autocad-interface/releases)

---
## Documentation

Documentation will be worked on throughout creation of tool.  

![Ribbon Menu](/Resources/Ribbon-menu.png "Ribbon menu")
Once loaded the following tools are available in the ribbon menu.

![Login screen](/Resources/Login-screen.png "Login screen")
Within settings the user can log in to their AGOL account and select the destination CRS.

![Loading Layers](/Resources/Loading-layers.png "Loading layers")
Layers can be selected by first choosing a parent folder to select from.

![Add Attribute](/Resources/add-attribute.png "Add attribute")
If the chosen block has an attribute, the feature layer's own attributes can be selected from to fill in the value of each block.

![Example](/Resources/example-loaded.png "Example")
Example of the boundary layer with comments.

---
## Future Work
<li>Enabling the user to load in local files instead of just AGOL layers - In the form of shape files, Geopackage.</li>
<li>Enabling interface with PostgreSQL/PostGIS databases with querying possibility.</li>
<li>Enabling use of public datasets within the tool - British lidar dataset, world 30m topo etc.</li>

---
## Contact

[HarryBM](mailto:harrybm@gwp.uk.com)
