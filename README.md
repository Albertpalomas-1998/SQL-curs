-- SQL request(s)​​​​​​‌​‌​​‌‌​‌‌‌​​‌‌‌​‌​‌​​‌‌‌ below
select g.name as genre,
avg(t.milliseconds) as averageduration

From
Genre g

Join track t on g.GENREID=t.GENREID

group by g.NAME

Order by Averageduration desc

Limit 5;
