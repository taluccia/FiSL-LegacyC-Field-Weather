# FiSL-LegacyC-Field-Weather


## Fire 

Fire year     | Field fire scar name    | Official fire Name or ID 
------------- | ----------------------- | ------------------------ 
2015	        | Aggie			              | Aggie Creek
2015	        | Manley			            | Baker
2015	        | Mt Prindle 1			      | U.S. Creek
2015	        | Tanana Road			        | Hay Slough
2019	        | BearFish			          | Bearnose Hill
2019	        | LittleYunBear		        | Bearnose Hill	
2019	        | Beaver	                | Canada FireID = 2019BC005		
2019	        | Ethel			              | Canada FireID = 2019MA014 
2019	        | Mt Prindle 2            | Cripple Creek
2019	        | FrozenFish	            | Frozen Calf		
2019	        | FrozenBlackCalf			    | Frozen Calf	
2019	        | FrozenCalf			        | Frozen Calf	
2019	        | Livengood	              | Hess Creek	
2019	        | Marr	                  | Marr
2019	        | MarrRock                | Marr
2019	        | PreacherPreach			    | Preacher Creek
2019	        | Shovel	                | Shovel	
2019	        | BigTractor			        | Tractor Trail 2
2019	        | Tractor			            | Tractor Trail 2
2020	        | Isom			              | Isom Creek
2021	        | Chena                   | Munson Creek




# Measuring Distance

Distances between field plots and the nearest unburned pixel and nearest part of the fire perimeter were calculated with the `sf` package and `geosphere` package. Unburned pixels were acquired from the dNBR image for each fire using a threshold of 0.5. Each pixel was converted to a point. The distance between each field plot and nearest unburned point was calculated three ways: 1) based on Cartesian coordinates, 2) based on a spheroid, and 3) based on an ellipsoid. For the distance to the edge (i.e., fire perimeter), fire perimeters were converted to points and then distance betweeen field plots and the nearst point on the edge was calculated three ways: 1) based on Cartesian coordinates, 2) based on a spheroid, and 3) based on an ellipsoid.

The `geosphere` package was used to measure distance from Latitude and Longitude on a spheroid and Latitude and Longitude on an ellipsoid. [Link to](https://cran.r-project.org/web/packages/geosphere/geosphere.pdf) `geosphere` package

## Other links on measuring distance
https://gis.stackexchange.com/questions/198900/difference-between-planar-and-euclidean-distance
https://gis.stackexchange.com/questions/308508/difference-between-geodetic-distance-and-great-circle-distance





