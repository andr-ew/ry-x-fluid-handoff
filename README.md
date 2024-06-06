# Ry X fluid background

this is a fluid dynamics-based background animation created for [ry-x.com](ry-x.com) by andrew c. shike, forked from https://github.com/PavelDoGreat/WebGL-Fluid-Simulation

## license

permission is granted to the recipient to use & distribute this source code in connection with the website of Ry X. all other rights reserved, please do not modify the source code for any reason other than to improve performance & stability across platforms.

## usage

the "day" and "night" html files demonstrate inclusion of the script in the two intended colorways.

in the context of a larger page, scrolling will likely look bad, I reccommend fixing the canvas element and gradually decreasing opacity of the canvas element based on the scroll position. for performance you may need to stop the animation loop or remove the canvas element when the opacity reaches zero (it's posably unneccesary, depending on the behavior of requestAnimationFrame).

## performance

performance has not been widely tested, as this is a WebGL based script performance may impact usability of the site on devices with less graphics capability – on these devices it would be best to display a static image instead (provided in `img/`). profiling may be possible, but an alternative solution would be to fallback to a static image if the framerate dips below a certain threshold (say, 20fps) for a prolonged period.
