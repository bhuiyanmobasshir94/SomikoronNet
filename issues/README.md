# Dataset Creation Issues and Concerns

### Augmentation issues

- Rotation to a certain degrees of an image might lead to a sign or digit to be changed or misinterpreted
  - Cases: 
      - Rotating a "Plus(+)" sign 45 degree clockwise or counterclockwise will result that sign to become "multiplication(x)" sign or vice versa
      - Rotating a divide sign to 90 degree would render it as non recognisable sign, also same can be said for rotating the sign for 45 degree as well
      - Although there is a difference between percentage and divide sign rotating either of them to 45 degree could render them identical.
