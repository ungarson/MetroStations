<img src="https://i.ibb.co/WnD42Vy/metrostations.png" width="200" alt="metrostations" border="0"></img>
# Metro Stations
JSONs of metro stations and lines.

<h2>Content:</h2>
1. <a href="#what-you-can-do">What you can do</a> <br>
2. <a href="#available-cities">Available cities</a> <br>
3. <a href="#cities-in-progress">Cities in progress</a> <br>
4. <a href="#docs">Docs</a> <br>
5. <a href="#usage">How to use</a> <br>
6. <a href="#work-in-progress">Future updates</a> <br>
7. <a href="#anything-missing">Anything missing?</a>

<h2 id="what-you-can-do">What you can do:</h2>
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
<h2 id="available-cities">Available cities:</h2>
<ul>
<li>Moscow</li>
<li>Saint-Petersburg</li>
</ul>
<h2 id="cities-in-progress">Cities in progress:</h2>
<ul>
<li>Beijing</li>
<li>Tokyo</li>
<li>Shanghai</li>
<li>Seoul</li>
<li>Guangzhou</li>
</ul>

<h2 id="docs">Docs:</h2>
<h3> Stations: </h3>

`Stations` is an array of objects with information about stations.

Fields in the very next table exist in every stations.json.

| Fields | Value | Meaning |
| ------------- | ------------- | ------------- |
| local_name  | String  | Local name of the station |
| geo_lat | String  | Latitude position |
| geo_lon | String  | Longitude position |
| line  | Number  | ID of the line |
| id | Number | ID of the station |
| intl_name | String | Name of the station in English |
| lineTransfers | Array\<Number> | Array with lines' IDs with which the station has the intersection |
| stationTransfers | Array\<Number> | Array with stations' IDs with which the station has the intersection |

Fields in the very next table exist only in some stations.json.

| Fields | Value | Meaning |
| ------------- | ------------- | ------------- |
| grade | Underground &#124; Elevated &#124; At-grade | Station's grade |
| platform_type | String | Platform type |

<h3> Lines: </h3>

`Lines` is an array of objects with information about lines.

Fields in the very next table exist in every lines.json.

| Fields | Value | Meaning |
| ------------- | ------------- | ------------- |
| local_name  | String  | Local name of the line |
| intl_name | String | Name of the line in English |
| color | String | Line's color |
| id | Number | ID of the line |
| lineTransfers | Array\<Number> | Array with lines' IDs with which the line has intersections |


<h2 id="usage">How to use:</h2>

<h3> Download this super-duper repository </h3>

> npm i metrostations

<h3> Use it in your JS code </h3>

> import {Moscow} from 'metrostations' <br />
> const MoscowStations = Moscow.stations <br />
> const MoscowLines = Moscow.lines <br />
> <br />
> // your code goes here... 🚇

<h2 id="work-in-progress">Future updates:</h2>
Except the <a href="#cities-in-progress">cities in progress</a> part, 
we also neeed to write tests: <br>
<ol>
<li>To check whether two stations intersect correctly</li>
<li>To check whether two lines intersect correctly</li>
</ol>
Also:
<ol>
<li>Write a function to get a station by its name/geoposition in each city module</li>
<li>Write a function to get a line by its name/color in each city module</li>
</ol>
<h2 id="anything-missing">Anything missing?</h2>
In case we forgot some station or a line, or if you noticed some inappropriate behavior,
create <a href="https://github.com/ungarson/MetroStations/issues">new issue</a>
<br>
<br>
You can also DM the Founder: <br>
- Telegram: <a href="https://t.me/ungarson">@ungarson</a><br>
- Instagram: <a href="https://www.instagram.com/daniilorain/">@daniilorain</a>
