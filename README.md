# Ship Race: Spain to Puerto Rico (1770)
A stop-motion animation depicts two ships, El Rey and El Colon, racing across three different routes to determine which journey is the fastest.

<img src="./ShipRace Spain to Puerto Rico, 1770 720p.gif" img alt = "ShipRace GIF"/>

## How It's Made:

**Tech used:** ArcGIS Pro

The file opens up with the interpolated ship paths being active showing each still of the ship moving along its path, to get the ships to animate properly several steps had to be made. The first step is defining a per-feature filter using range. A range filter connects to any numeric field and will interactively filter features in the map. The range filter will be connected to the Hours_Travelled field, which indicates how long it has been since the ship left port. By stepping through individual feature locations one at a time and synchronizing the steps with the exported video frames, you will create the illusion of a ship moving across the ocean. In Bookmarks, I went to the Race Across Atlantic Bookmarks section and selected the Starting Line Bookmark. On the Logged Positions layer in the Contents pane, I went on Properties to add range, for the Start Field I chose HOURS_TRAVELLED. I did the same exact process for the Interpolated Positions layer, adn after doing the whole process a slider appears on the right side of the view and a Range tab appears on the ribbon, however, the filter is not actively applied which I clicked the Range Disabled button to enable it. On the Range tab, in the Current Range group, I set the Max to 24 and Span to 0. Because the span is 0, the minimum value updates to 24 to match the maximum value. The minimum value means 24 hours into the journey, or after one day at sea. The span value of 0 means one slice of data. A span of 10, for example, would show 10 hours of content, and you would see multiple ships. Then in the Strp group, I clicked the Use Range SPan button and for the Step Interval inserted 2.




## Lessons Learned:

No matter what your experience level, being an engineer means continuously learning. Every time you build something you always have those *whoa this is awesome* or *wow I actually did it!* moments. This is where you should share those moments! Recruiters and interviewers love to see that you're self-aware and passionate about growing.

## Repositories
**Profile:** [T3ch12et](https://github.com/T3ch12et)

**Cartography Repository:** [ESRI MOOC Cartography](https://github.com/T3ch12et/GIS-Data-Science-Portfolio/tree/main/ESRI-MOOC-Cartography)

**Main Repository:** [GIS Data Science Portfolio](https://github.com/T3ch12et/GIS-Data-Science-Portfolio)

## Examples:
Take a look at these couple examples that I have in my own portfolio:

**Miami Sea Level Rise:** [3D Miami Beach Sea Level Rise](https://github.com/T3ch12et/GIS-Data-Science-Portfolio/tree/main/ESRI-MOOC-GIS-for-Climate-Action/3D-Miami-Beach-Sea-Level-Rise)

**Athens Heat Risk Index:** [Athens Heat Risk Index](https://github.com/T3ch12et/GIS-Data-Science-Portfolio/tree/main/ESRI-MOOC-GIS-for-Climate-Action/Athens-Heat-Risk-Index)

**Oso Mudslide:** [Oso Mudslide](https://github.com/T3ch12et/GIS-Data-Science-Portfolio/tree/main/ESRI-MOOC-Cartography/Oso-Mudslide)

**Hurricanes since 1851:** [Hurricanes since 1851](https://github.com/T3ch12et/GIS-Data-Science-Portfolio/tree/main/ESRI-MOOC-Cartography/Hurricanes-since-1851) 

**Coral Reef Dashboard:** [Coral Reef Dashboard](https://github.com/T3ch12et/GIS-Data-Science-Portfolio/tree/main/ESRI-MOOC-GIS-for-Climate-Action/Coral-Reef-Dashboard)

**Rondonia Land Cover Change:** [Rondonia Land Cover Change from 1992 to 2020](https://github.com/T3ch12et/GIS-Data-Science-Portfolio/tree/main/ESRI-MOOC-GIS-for-Climate-Action/Rondonia-Land-Cover-Change)

**Addressing Climate Change:** [Using GIS to address climate change](https://github.com/T3ch12et/GIS-Data-Science-Portfolio/blob/main/ESRI-MOOC-GIS-for-Climate-Action/Addressing-Climate-Change/README.md)

**Shipping in 1770:** [World Shipping in 1770](https://github.com/T3ch12et/GIS-Data-Science-Portfolio/tree/main/ESRI-MOOC-Cartography/Shipping-in-1770)
