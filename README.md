# Tableau Dashboards folio

Tableau Projects/Workbooks/Dashboards that I developed for learning.

Check out my portfolio at : [tableau.com/mansi.rajesh.borole5345](https://public.tableau.com/app/profile/mansi.rajesh.borole5345)
and Certification! [https://www.credly.com/badges/79049684](https://www.credly.com/badges/79049684-8d6d-499b-829f-0fa615129fcb/public_url)

# Level of Detail Calculations (create more dynamic visualizations):
[Tableau Public link | Netflix Movies & TV Shows Analysis >>](https://public.tableau.com/app/profile/mansi.rajesh.borole5345/viz/NetflixMoviesTVShowsAnalysis_16750004131640/NetflixDashboard)

[Tableau Public link | Credit Card Complaints Dashboard >>](https://public.tableau.com/app/profile/mansi.rajesh.borole5345/viz/CreditCardComplaintsDashboard_16753553405910/Dashboard1)

Level of detail (LOD) calculations allows to aggregate data at different levels of granularity and provide a way to calculate results based on dimensions that are not in the view. . LOD expressions provide a way to perform calculations that are not based on the dimensions in the view, and allow you to isolate specific dimensions and measure combinations.

To get the last 12 months dates from today we need to make a simple LOD calc: 

DATEDIFF('month',DATETRUNC('month',[Date received]),
DATETRUNC('month',[Parameters].[Max Date Received])
)<12
![Netflix Dashboard](https://user-images.githubusercontent.com/31558571/216674694-4bec1b02-ad14-4379-bf29-58a6247a00e0.png)

# Sparkline

Make dual Axis
Synchronize axes
Make one chart area
Make a second chart line

# Progress bar

create a calculated field (0-100%)
add it to a columns card
create another field to represent 100 % - can use avg(1) -this will be the background of the progress bar!
add it to the columns card
create a dual axis, synchronize and hide the legends

# Dynamic Calculations

Using parameters in calculated fields
![Credit Card Complaints Dashboard](https://user-images.githubusercontent.com/31558571/216674783-4f7fc4d0-16a2-4dee-a8e8-0cac34e671f1.png)

# Density Maps

[Tableau Public link | AirBnb Listings Density Maps](https://public.tableau.com/app/profile/mansi.rajesh.borole5345/viz/AirBnbListingsDensityMaps/Sheet1)

1. Double click **Latitude and Longitude**.
2. Add the **id** to the **Details**
3. Select “Density” in the **Marks**
4. Modify **Density / Opacity** options in the **Color**
5. Create a parameter containing years from 2008 to 2019.
6. Create a field having formula **YEAR([Host Since]) <= [Parameters].[Year].**
7. Show the parameter and set it up as **Slider**.
![AirBnb Listings_ Density Maps!](https://user-images.githubusercontent.com/31558571/216675721-14c0275f-cba7-4a8d-8c0a-f1b79d290e4e.png)


# Butterfly Charts

[Tableau Public link | Adult Literacy Butterfly charts >>](https://public.tableau.com/app/profile/mansi.rajesh.borole5345/viz/AdultLiteracyButterflycharts/Sheet1)

Usually used for gender based data and the axis is usually a discrete dimension. Eg. name of districts in our case

1. add the Districts dimension to rows
2. add the make and female literacy rates to the columns
3. create a zero axis , this will be the center axis of our chart. use a calculated field, and in the formula enter 0
4. place the zero axis in between the male and female columns. Add the district labels to it
5. Reverse the axis on the left
![Adult Literacy (Butterfly charts)](https://user-images.githubusercontent.com/31558571/216674644-dff55eca-aa65-4290-a096-99b013787cd1.png)

# Exporting to PDF/ JPEG/ Crosstab/ PPT
1. Drag the download object in the dashboard layout
2. Use the edit button options to configure the action to download as PDF/ JPEG/ Crosstab/ PPT
