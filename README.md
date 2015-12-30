# Where Is the Sun

Utilities for converting between various coordinate systems for tracking the position of the sun in the sky.

The coordinate systems I plan to include are:
* Equatorial 
* Altitude Azimuth
* Cone Azimuth

The code will be in JavaScript. You're probably wondering why anyone would use JavaScript to track the sun. Well, it seems some folks are using JavaScript for robotics via [Johnny Five](http://johnny-five.io/), so maybe someone will find this useful.

### What is 'Cone Azimuth'?
(I coined this term because I don't know what this coordinate system is called by others.)

Cone Azimuth is a coordinate system where the altitude vector lies along a cone. It is easier to see an example than to read a discription of this. The most famous example of a system that utilizes this coordinate system is the done of the [Thirty Meter Telescope](http://www.tmt.org/) (TMT). The opening of the dome rises and falls according to the rotation of a circular portion that lies at an angle to the rest of the dome. (The main benefit of this sort of dome is that it permits the smallest opening on the dome for the telescope aperture; for a telescope as large as the TMT, an excessively large dome aperture can threaten the integrity of the dome, or so I hear.) Because the rotation of the altitude along a cone also changes its azimuth, this needs to be compensated for in the azimuth coordinate of the cone itself. Additionally, an cone azimuth coordinate system gives you two coordinate possibilities for each point in the sky. Only points along the horizon have one coordinate possibility.  

Why am I including cone azimuth? Who even uses this? Nobody yet, as far as I know. I have some ideas for this that I may want to build in the future; I may as well prepare the code for it now.
