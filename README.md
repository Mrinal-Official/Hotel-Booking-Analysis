# Hotel Booking Exploratory Data Analysis
## Obective:
I have Hotel Booking dataset.The main objective of this project is explore the given dataset and find useful conclusion about general trends in hotel booking and discover how these factors affect on hospitality business.
## Dataset:
The iven dataset have information of city and resort hotel. This dataset have 11390 rows and 32 coulumns. The columns from the dataset is as follows:

**Hotel:** Type of hotel(City or Resort)

**is_cancelled:** If the booking was cancelled(1) or not(0)

**lead_time:** Number of days before the actual arrival of the guests

**arrival_date_year:** Year of arrival date

**arrival_date_month:** Month of arrival date

**arrival_date_week_number:** Week number of year for arrival date

**arrival_date_day_of_month:** Day of arrival date

**stays_in_weekend_nights:** Number of weekend nights(Saturday or Sunday) spent at the hotel by the guests.

**stays_in_weel_nights:** Number of weeknights(Monday to Friday) spent at the hotel by the guests.

**adults:** Number of adults among the guests

**children:** Number of children

**babies:** Number of babies

**meal:** Type of meal booked

**country:** country of the guests

**market_segment:** Designation of market segment

**distribution_channel:** Name of booking distribution channel

**is_repeated_guest:** If the booking was from a repeated guest(1) or not(0)

**previous_cancellation:** Number of previous bookings that were cancelled by the customer prior to the current booking

**previous_bookings_not_cancelled:** Number of previous bookins not cancelled by the customer prior to the current booking

**reserved_room_type:** Code from room type reserved

**assigned_room_type:** Code of room type assigned

**booking_changes:** Number of changes made to the booking

**deposit_type:** Type of deposite made by the guest

**agent:** ID of travel agent who made the booking

**comapny:** ID of the company that made the booking

**days_in_waiting_list:** Number of the days the booking was in the waiting list

**customer_type:** Type of customer, assuming one of four categories

**adr:** Average daily rate

**required_car_parking_spaces:** Number of car parking spaces required bt the customer

**total_of_special_requesrs:** Number of special requests made by the customer

**reservation_statuse:** Reservation status(Canceled, check-out or no-show)

**reservation_status_date:** Date at which the last reservation status was updated
## Data cleaning and manipulation:
## **Duplicate values**
Dataset have 31994 duplicate values. so these duplicate values are removedfrom dataset using.drop_dupliactes(). After droping duplicate value shape of the dataset become 87396 rows and 32 columns.
## **Missing values/null values**
Given dataset have 4 columns company, aent, country and children missing values so these values are replace by usin .fillna() function.
## **Adittion of new columns**
Total_people and Total_stay these two columns are added in given dataset
Some rows are removed from columns adults, children and babies.
## EDA:
The EDA is done by using 3 analysis Univariate, Bivariate and Multivariate analysis. For the datavisualization following charts are used:

Pie chart

Barplot

Countplot

Heatmap

### Univariate analysis:
**In univariate analysis following questions are tried to solve:**
1) Which type of hotel is mostly prefered by the guests?
2) Which agent made the most bookings?
3) What is the percentage of repeated guests?
4) What is the most preferred room type by the customers?
5) What type of food is mostly prefered by the guests?
6) In which month most of the bookings happened?
7) Which distribution channel is mostly used for hotel booking?
8) which year had highest bookings?
     
## Conclusion:
1) City hotel has more bookings.
2) Agent no. 9 made most of the bookings.
3) There are very few guests booking for the same hotel again.
4) A type rooms are most prefered rooms.
5) BB type food is most preferred food.
6) August month has maximum number of bookings.
7) Mostly used distribution channel is TA/TO channel.
8) 2016 has highest bookings.
### Bivariate and Multivariate analysis:
**In bivariate and multivariate analysis following questions are tried to solve:**
1) Which hotel type has the highest ADR?
2) which hotel has longer waiting time?
3) Which distribution channel contributed more to adr in order to increase the income?
4) What is optimal stay length in both types of hotel?
5) Relationship between the repeated guests and previous bookings not canceled?
6) Relationship between ADR and total number of people?

## Conclusion:
1) City hotel has highest adr.
2) City hotel has longer waiting time.
3) GDS distribution channel contributed more to ADR in city hotel.
4) Optimal stay length in both hotel type is less than 7 days.
5) Repeated guests do not cancel there bookings.
6) Number of people increases adr aslo going to increase.

### Conclusion from correlation heatmap
1) arrival_date_year and arrival_date_week_number columns has negative correlation which is -0.51.
2) stays_in_week_nights and total_stay has positive correlation which is 0.95.

## Overall conclusion:
1) City hotel has almost 60% bookings and resort hotel has 40% bookings.
2) Agent no. 9 made most bookins and those bookings are 28721.
3) Percentage of repeated guest is just 4%.
4) Room type A is most preferred room type 46283 guests preferred A room type.
5) BB type food is most preferred food type and 67907 preferred this food.
6) Auust month has maximum number of bookings and those bookings are 11242.
7) TA/TO distribution channel is mostly prefderred channel and the bookings are 69028.
8) 2016 year has 42313 bookings.
9) City hotel has highest ADR and trhe average ADR is 111.27.
10) City hotel has longer waiting time means city hotel is busy hotel type.
11) GDS contribution channel contributed more to ADR in order to incerease income in city hotel.
12) Optimal stay length in both hotel type is leaa than 7 days.
13) Repeated do not cancel there bookings.
14) The number of people increases ADR increases.
15) arrival_date_year and arrival_date_week_number columns has negative correlation which is -0.51.
16) stays_in_week_nights and total_stay has positive correlation which is 0.95.
