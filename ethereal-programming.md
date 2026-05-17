# Ethereal Programming
## Variables `h,u,z`
The Etherreal can be thought of as a sphere, where we have longitude, latitude, and radius. However the three listed variables (`h,u,z`) are not immediately related to the longitude, latitude, or the radius instead they are related to actual prime and entrophic elements themselves.

	Prime elements:
		`h` = heft (the earth(+)/air(-) scale)
		`u` = energy (the fire(+)/water(-) scale)
	`z` = entrophic elements (positve(+)/negative(-) scale)
	
### Longitude
```
o = atan2(h,u)
```
### Latitude
```
r_p = sqrt(h^2 + u^2)
l = atan(r_p / z)
```
### Distance
```
r = sqrt(r_p^2 + z^2)
```

## Formula
E(t,h,u,z) = r sin(ot + l)
