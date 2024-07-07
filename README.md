# Ship Race: Spain to Puerto Rico (1770)
A stop-motion animation depicts two ships, El Rey and El Colon, racing across three different routes to determine which journey is the fastest.

<img src="./ShipRace Spain to Puerto Rico, 1770 720p.gif" img alt = "ShipRace GIF"/>

## How It's Made:

**Tech used:** ArcGIS Pro

The file opens up with the interpolated ship paths being active showing each still of the ship moving along its path, to get the ships to animate properly several steps had to be made. The first step is defining a per-feature filter using range. A range filter connects to any numeric field and will interactively filter features in the map. The range filter will be connected to the Hours_Travelled field, which indicates how long it has been since the ship left port. By stepping through individual feature locations one at a time and synchronizing the steps with the exported video frames, you will create the illusion of a ship moving across the ocean. In Bookmarks, I went to the Race Across Atlantic Bookmarks section and selected the Starting Line Bookmark. On the Logged Positions layer in the Contents pane, I went on Properties to add range, for the Start Field I chose HOURS_TRAVELLED. I did the same exact process for the Interpolated Positions layer, adn after doing the whole process a slider appears on the right side of the view and a Range tab appears on the ribbon, however, the filter is not actively applied which I clicked the Range Disabled button to enable it. On the Range tab, in the Current Range group, I set the Max to 24 and Span to 0. Because the span is 0, the minimum value updates to 24 to match the maximum value. The minimum value means 24 hours into the journey, or after one day at sea. The span value of 0 means one slice of data. A span of 10, for example, would show 10 hours of content, and you would see multiple ships. Then in the Strp group, I clicked the Use Range SPan button and for the Step Interval inserted 2.

The next step is the use the range filter to create a stop-motion animation. I needed to create exactly one image, or frame, in the final video for each defined position of the ships. I zoomed to the Starting Line bookmark, ensuring that the range slider is reset to the beginning of the range, then I opened the Animation Timeline pane and created the first keyframe to the animation. Before adding the rest of the keyframe, I set the append time which will create an animation that shows 25 individual states of the range slider per second. Next up is to import the rest of keyframe from the range slider steps. Importing the range steps and setting the append time will create an animation with 422 keyframes, one for each two-hour step through the range slider, with a current total playing time of about 16.8 seconds. The end goal for the animation output is to be in Youtube format.

Now that I have those steps in tow, I have to update the last keyframe to show the end of the race. I currently selected the 422nd keyframe, which is the last frame, to get the camera setup the way I want it. The last keyframe is when the slowest ship arrives. You need the camera to get to the finish line when the fastest ship arrives, and then hold the same viewpoint until all the ships finish. The data shows that the winner arrives after 29 days of travel, which means that there were 348 (29 x 12) range slider steps for it to arrive. The arrival keyframe, therefore, is #349. I zoomed to keyframe 349 and then zoomed to the Finish Line bookmark and clicked Update on the Animation tab in the Edit group. I zoomed to the Racetrack bookmark to verify the camera path which shows a straight line that doesn't keep the ships in view.




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
