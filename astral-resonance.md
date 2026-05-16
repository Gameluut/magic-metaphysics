# Astral Resonance
## Variables
The Astral Plane is like a coordinate plane for the different aignments where you have an axis for good/evil and another axis for law/chaos, thus we end up with two variables: `m` (morality for the good/evil axis and will act as the y-axis) and `s` (structure for the law/chaos axis and will act as the x-axis).
### Geometry of the Astral plane
Because of the design of the Astral plane, the 2d coridnate system of the astral plane becomes warped when brought into a 3d space and the four corners move. We end up with a structure where LE `(+,-)` and CG `(-,+)` are closer to TN (0,0) than LG `(+,+)` and CE `(-,-)`. Thus we can make a formula to calculate how far any alignment is from TN with the formula `d = |2m| + |s|`
#### Resonance Coordinates
The alignment does not create the resonance in a straight forward manner. Instead we will have to take into consideration how well different alignments interact with the entrophic (positive/negative) elements
##### Interactions with the entrophic elements.
Good alignments tend to interact much more agreeably with the positive element while evil alignments tend to interact much more agreeably with the negative element. However, the negative element shows a slight preference for lawful alignments while the positive element shows a slight preference for chaotic alignments. Using this we can create a formula to find an interaction quotient
```
#+ value is better with the positive element
#- value is better with the negative element
q = 3m - s
```
##### Transfering Resonance onto a new "unwarped" plane
Modifying the `d` formula so `d'= 2m + s` instead, we can use `q` and `d'` to find the new axis we will want to use by making `q = d'`resulting in the fromula `2m + s = 3m - s` which simplifies to `2s=m` giving us a new axis moving at approximately 26.57° (0.4636 rad) or `arctan(.5)` above the `m` axis.
## Formula
