# Season Tracking
 I wanted to look into when British seasons actually start.  Officially, each season is three months long, starting in line with the equinoxes, so 20th March -> 21st June -> 22nd September -> 21st December.
 That didn't seem right to me though, I felt winter started at the beginning of December and surely summer starts before the end of June?  So, I decided to look at the data.
 
 ## The Data
 I downloaded data from the CEDA archive (https://data.ceda.ac.uk/badc/ukmo-midas-open) that covered temperatures, wind, and rain.
 
 ## The Process
 I started with the view that the start of summer should be defined as the beginning of the hottest 90 day window, simmilarly the start of winter should be the start of the coldest 90 day window.
 I resampled the data into daily observations and ran 90 day rolling windows to get the mean observations for each window.  Then, for each year I found the minimum and maximum date:value pairs for temperature high & lows, driest and wettest, and windest and calmest days.  With these I was able to create histograms and kernel density estimates for when the seasons have most often started.
 
 ## Results
 ![Results](https://github.com/angus-93/Season-Tracking/files/6725633/90_day_window_plot.pdf)

