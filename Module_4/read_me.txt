select
    city
from
    dst_project.airports
group by 
    city
having
    count(airports.latitude/airports.longitude) > 1 
order by 
    city
