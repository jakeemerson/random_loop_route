# Random Loop Routes

For a little side project I was interested in finding a way to create random routes for exploring a place. When traveling it's usually easiest to follow guidebooks or Google searches to find places to explore. However, this will only lead you to popular places. Even near home it's comfortable to stay on the familiar routes. But what if the familiar is getting tiresome? Perhaps there is an interesting garden to see out there, or a nice park that you have never noticed before. Randomness to the rescue!

This repo holds a single Jupyter notebook with some initial work on this problem. I was surprised to find that there isn't much available on the web for examples of how to produce random loops for exploring an area. The approach that I took was to start with a random starting location, which could be constrained by a bounding box, and draw a circle around it that has a circumference roughly equal to how far I want to walk or bike (in kilometers). Then connect four paths around this circle for my randomly generated route.

There are clearly issues to still work out or criteria to add, such as:

- minimize the number of turns
- limit any back-tracking along the tour
- don't go down cul-de-sac streets
- start from a specific location and route to the nearest point on the loop

The notebook here shows a nice little example of a ~10km tour in Berlin, Germany. Enjoy!

## Installing

Prior to running `pip install -r requirements.txt` be sure to install the `rtree` package as described here: http://toblerity.org/rtree/install.html
