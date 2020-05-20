# Reason for forking:

## Android:

* Landscape / portrait is not correctly detected (it's just checking width/height, not transform).
    - Adding 'rotationDegrees' to load event, so we can correctly calculate video dimensions.
    
## IOS
     
* Load event:
    - TODO: Add a more in depth explanation on what was wrong with the old preferredTransform check, and what we solve with our new fix...
    - Wrongly checks preferred transform for whether it's landscape or portrait. 
    -  Also width/height was not set depending on preferred transform, so video got wrong dimensions. 


