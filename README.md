<img src="https://i.ibb.co/WnD42Vy/metrostations.png" width="200" alt="metrostations" border="0"></img>
# Metro Stations
JSONs of metro stations and lines.

### Content:
1. [What you can do](#what-you-can-do)
2. [Available cities](#available-cities)
3. [Usage](#usage)
4. [Anything missing?](#anything-missing)

<h3 id="what-you-can-do">What you can do</h3>
<ul>
<li>Get list of almost all the lines</li>
<li>Get list of almost all the stations</li>
<li>Get latitude and longitude of available stations</li>
<li>Get the color of a line</li>
<li>Check whether two selected stations intersect</li>
<li>Check whether two selected lines intersect</li>
</ul>

Why almost all the lines and stations? 

For example, let's consider the Moscow case: they have monorail,
which is not really a part of Metro system, 
and they also have MCD, which is also not really a part of the metro system. <br>
So, in the case of Moscow we don't include neither monorail nor MCD.
<h3 id="available-cities">Available cities</h3>
- Moscow

<h3 id="usage">Usage</h3>

> npm i metrostations

and then use it in the code:

> import {Moscow} from 'metrostations' <br />
> const MoscowStations = Moscow.stations

<h3 id="anything-missing">Anything missing?</h3>
In case we forget some station or a line, or you noticed some inappropriate behaviour,
create <a href="https://github.com/ungarson/MetroStations/issues">new issue</a>
<br>
<br>
You can also DM the Founder: <br>
- Telegram: <a href="https://t.me/ungarson">@ungarson</a><br>
- Instagram: <a href="https://www.instagram.com/daniilorain/">@daniilorain</a>