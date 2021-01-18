# Dataset Creation Issues and Concerns

### Augmentation issues

  - Rotation to a certain degrees of an image might lead to a sign or digit to be changed or misinterpreted
    - Cases: 
      - Rotating a "Plus(+)" sign 45 degree clockwise or counterclockwise will result that sign to become "multiplication(x)" sign or vice versa
      - Rotating a divide sign to 90 degree would render it as non recognisable sign, also same can be said for rotating the sign for 45 degree as well
      - Although there is a difference between percentage and divide sign rotating either of them to 45 degree could render them identical.
      - Not in general but rotating an image containing bangla 8 could be misidentified as bangla 7
    - Stretch/Compress
      - When in congestion the writtings may overlap seemingly and could become ambiguous to machiner
      - Streching certain bangla numerics can lead to ambiguity such as bangla five has possibility of becoming bangla 0 and vice versa
      - A lot of cases stretching image could lead an image to become bloated and in case of "divide sign" the upper and lower dot could easily become a line leading to probable misidentification chance
      - Stretching first bracket can lead that to become curly brackets/second brackets and compressing could made it third/square brackets or vice-versa

### Variation
  - Since we will be dealing with hand writting and it differs from person to person it is possible that variation of a certain or all the target classes is so high that the machine becomes unable to draw a decision boundary among them
  - Different people have different ways of writting each numbers so the greater the database(considering how many people have contributed) the greater will be the variation

### Info 
- since object recognition from image is basically the checks of pixel value in an image and making a decision boundary, a issue in english hand written number recognition states that hand written numerical/non-numerical value could have so variation that it could become almost impossible to identify them (1). So they introduced a line based approach. (1)

### Misc.
- written form of bangla 1, 5 and 0 has a lot similarities and may lead misidentification
- A lot of cases bangla 3 and 0 can be misindentified as a little stretch at the end of 3 and a not fully closed 0 may become same
- Since we are using bangla "of" known as "er" the first letter has a similarity with bangla 3 which could be misinterpretated easily
- If the images/samples is of very low quality then the machine will lose a great deal of knowledge because the signs are very similar to one another
- If the images have very low resolution then it may become impossible for the machine to correctly identify

### References
1. https://medium.com/bethgelab/ai-still-fails-on-robust-handwritten-digit-recognition-and-how-to-fix-it-a432d84ede18
