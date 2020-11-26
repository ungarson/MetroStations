<img src="https://i.ibb.co/WnD42Vy/metrostations.png" width="200" alt="metrostations" border="0"></img>
# Metro Stations
JSONs of metro stations and lines.

<h2>Content:</h2>
1. <a href="#what-you-can-do">What you can do</a> <br>
2. <a href="#available-cities">Available cities</a> <br>
3. <a href="#cities-in-progress">Cities in progress</a> <br>
3. <a href="#usage">Usage</a> <br>
4. <a href="#work-in-progress">Work in progress</a> <br>
5. <a href="#anything-missing">Anything missing?</a>

<h2 id="what-you-can-do">What you can do</h2>
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
<h2 id="available-cities">Available cities</h2>
<ul>
<li>Moscow</li>
<li>Saint-Petersburg</li>
</ul>
<h2 id="cities-in-progress">Cities in progress</h2>
<ul>
<li>Beijing</li>
<li>Tokyo</li>
<li>Shanghai</li>
<li>Seoul</li>
<li>Guangzhou</li>
</ul>

<h2 id="usage">Usage</h2>

> npm i metrostations

> import {Moscow} from 'metrostations' <br />
> const MoscowStations = Moscow.stations <br />
> const MoscowLines = Moscow.lines

<br>
<h2 id="work-in-progress">Work in progress</h2>
Except the <a href="#cities-in-progress">cities in progress</a> part, 
we also neeed to write tests: <br>
<ol>
<li>To check whether two stations intersect correctly</li>
<li>To check whether two lines intersect correctly</li>
</ol>
<br>
<h2 id="anything-missing">Anything missing?</h2>
In case we forgot some station or a line, or if you noticed some inappropriate behavior,
create <a href="https://github.com/ungarson/MetroStations/issues">new issue</a>
<br>
<br>
You can also DM the Founder: <br>
- Telegram: <a href="https://t.me/ungarson">@ungarson</a><br>
- Instagram: <a href="https://www.instagram.com/daniilorain/">@daniilorain</a>