# Variables
The Astral Plane is like a coordinate plane for the different aignments where you have an axis for good/evil and another axis for law/chaos, thus we end up with two variables: `m` (morality for the good/evil axis and will act as the y-axis) and `s` (structure for the law/chaos axis and will act as the x-axis).

## Geometry of the Astral plane
Because of the design of the Astral plane, the 2d coridnate system of the astral plane becomes warped when brought into a 3d space and the four corners move. We end up with a structure where LE `(+,-)` and CG `(-,+)` are closer to TN (0,0) than LG `(+,+)` and CE `(-,-)`. Thus we can make a formula to calculate the distance from TN as follows:
```
# Magnitude
d = sqrt(4m^2 + s^2)
# Direction
k = atan2(2m,s)
```
### Resonance Coordinates
The alignment does not create the resonance in a straight forward manner. Instead we will have to take into consideration how well different alignments interact with one the entrophic (positive/negative) elements
#### Interactions with the entrophic elements.
Good alignments tend to interact much more agreeably with the positive element while evil alignments tend to interact much more agreeably with the negative element. However, the negative element shows a slight preference for lawful alignments while the positive element shows a slight preference for chaotic alignments. Using this we can create a formula to find an interaction quotient
```
#+ value is better with the positive element
#- value is better with the negative element
q = 3m+s
```
####
Now we use the new `q` value to create a new y-axis. However we will also need a new x-axis that runs perpendicular to out `q` value. Let's call this new value `p`. However, the distance of `q` and `p` (`D = sqrt(q^2 + p^2)`) must equal `d.` and thus we end up with the following calculation for p.
```
r = 6ms - 5m^2 #this is a temporary var
p = sgn(r) sqrt(|r|)
```