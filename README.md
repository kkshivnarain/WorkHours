# WorkHours
Python pandas based time difference calculation in business hours

Installation
Direct Download from https://github.com/kkshivnarain/WorkHours/archive/0.2.tar.gz



Sample code
from WorkHours import WorkHours
wh=WorkHours() #initialize the WorkHours class
wh.holiday_calendar("2017/7/3") #Define holidays one at a time 
wh.business_hours(8,18,'01234') #Define standard shift hours e.g 8:00 to 18:00 Hours everyday from Monday to Friday
wh.working_calendar("2017/7/24","2017/7/31") #creating work calendar for defined business hours and holidays for a given date range
wh.business_hour_diff("07/24/2017 17:00:00","07/25/2017 08:00:00")  #example for calculating time difference- it should return 1 hour
