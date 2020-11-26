<img src="https://i.ibb.co/WnD42Vy/metrostations.png" width="200" alt="metrostations" border="0"></img>
# Metro Stations
JSONs of metro stations and lines.
### What you can do:
- Get list of almost all the lines
- Get list of almost all the stations
- Get latitude and longitude of available stations
- Get the color of a line
- Check whether two selected stations intersect
- Check whether two selected lines intersect

Why almost all the lines and stations? 

For example, let's consider the Moscow case: they have monorail,
which is not really a part of Metro system, 
and they also have MCD, which is also not really a part of the metro system.
So, almost.
### Available cities
- Moscow
### Usage
> npm i metrostations
>
and then use it in the code:
> import {Moscow} from 'metrostations' <br />
> const MoscowStations = Moscow.stations
>