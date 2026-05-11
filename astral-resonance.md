# Variables
The Astral Plane is like a coordinate plane for the different aignments where you have an axis for good/evil and another axis for law/chaos, thus we end up with two variables: m (morality for the good/evil axis and will act as the y axis) and s (structure for the law/chaos axis and will act as the x axis). For the sake of this formula let's give both of these numbers a range of `(-1,1)`

## Geometry of the Astral plane
Because of the design of the Astral plane, the 2d coridnate system of the astral plane becomes warped when brought into a 3d space and the four corners move. We end up with a structure where LE `(1,-1)` and CG `(-1,1)` are closer to TN (0,0) than LG `(1,1)` and CE `(-1,-1)`. Thus we can make a formula to calculate the distance from TN as follows:
```
# Magnitude
d(m,s) = sqrt(4m^2+s^2)/3
# Direction
k(m,s) = atan2(2m,s)
```
### Interactions with the positive & negative elements.
Good alignments tend to interact much more agreeably with the positive element while evil alignments tend to interact much more agreeably with the negative element. However, the negative element shows a slight preference for lawful alignments while the positive element shows a slight preference for chaotic alignments. Thus we can make a formula to figure out how well each alignment will interact with the two different positive and negative elements.
```
#+ will interact better with the positive element, - will interact better with the negative element
q(m,s) = atan(3m,-s)
```
###
