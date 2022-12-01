# project-3-sli

This is a web page for the CS424 project 3.
1.	README.md (this file): This file provides information about the dataset, questions, data transformations, encodings, findings, and interactions.
2.	A bunch of source codes and data files were used in this project.
3.	The web page hosting your visualization interface: https://chloelili22.github.io/index.html
4.	A jupyter file includes the code for processing data from Chicago Data Portal.
This project is to build a web-based visualization host with single-linked view interactive plots, multiple-linked views interactive plots from previous projects, and additional multiple-lined views and new spatial views. 
In our project, the dataset is Taxi Trips in March, June, and September 2021 from Chicago Portal. We accessed CSV data from Chicago Data Portal and processed them via jupyter to clean, sort, and remove attributes of data as we needed. Besides the dataset, we encoded the visualizations and host them on the GitHub page with JavaScript and HTML. Inside the HTML and JavaScript, we mainly imported the d3.js library to produce interactive data visualization.
Based on the taxi trips in March, June, and September, we come up with 4 questions as follow:
1. Comparing the taxi trips in March with June and September, which taxi company is more favorable in fare?
2. Based on the distribution of the top 20 tips of trips in three months, how do taxi trips distribute in Chicago?
3. Comparing the taxi trips in March with June and September, which taxi company has better service based on tips distribution?
4. Based on the distribution of fares and timeline in March, June, and September, which taxi trips cost the most?
Firstly, we took a reference from a previous project to create three scattered and interactive plots representing the distribution of taxi trips based on distance and fare. By brushing the plots, the user can see the text field displaying the information about the trip by selecting dots. The companies with longer distances and lower fares were Taxi Affiliation Services, Taxicab Insurance Agency, LLC, and Taxicab Insurance Agence, LLC in March, June, and September in Figures 1, 2, and 3.  
![image](https://user-images.githubusercontent.com/80800544/204972452-2c096b10-fa86-4260-9de5-6038bdd65b24.png) 
Figure 1. Single view interactive plot of taxi trips in March

![image](https://user-images.githubusercontent.com/80800544/204972478-19f9a438-e304-442d-a425-2922c949fe32.png)
Figure 2. Single view interactive plot of taxi trips in June

![image](https://user-images.githubusercontent.com/80800544/204972519-cb8b86c7-3aa1-4a25-a1c6-99ef23e19fd1.png)
Figure 3. Single view interactive plot of taxi trips in September

Secondly, we created a spatial visualization with taxi trips and a leaflet library. We removed the taxi trips with duplicate coordinates and sorted data based on tips in descending order. We took the top 20 taxi trips and made markers on the map. Zooming on the map clearly displays the distribution of taxi trips in the Chicago area in Figure 4. To classify the trips in different months, red, green, and blue markers are taxi trips from March, June, and September. Since there were some coordinates of trips duplicated with other trips in different months, the markers will overlap with other trips from other months, which is not exactly 20 markers for each month in the graph. In light of this plot, there was a higher density of pedestrians in the downtown loop and lakeshore areas in Chicago. 
![image](https://user-images.githubusercontent.com/80800544/204972562-2b04a5ef-34de-42ae-918f-8585c900e2c5.png)
Figure 4. Distribution of top 20 trips in March, June and September
Meanwhile, there were two taxi trips to O’Hare airport. Pointing to the markers, we can see more info about those trips in Figures 5 and 6. The taxi company Flash Cab was more expensive than Taxi Affiliation Service. However, Taxi Affiliation Service achieved higher tips.
![image](https://user-images.githubusercontent.com/80800544/204972578-a699c69c-782b-4805-97f9-0a661f935fd1.png)
Figure 5. Comparison between two trips in O’Hare Airport.
![image](https://user-images.githubusercontent.com/80800544/204972599-29cb5bfe-337c-4ee4-82e2-609b2c044976.png)
Figure 6. Comparison between two trips in O’Hare Airport.
In addition, we also port three multiple linked views from the previous project. Three interactive visualizations represent the tips distribution of taxi trips in March, June, and September. The bar char represents the number of trips and taxi companies from the scattered plot. As the default state, the companies have the most trips in March, June and September were Flash Cab, Flash Cab, and Taxi Affiliation Service.  
![image](https://user-images.githubusercontent.com/80800544/204972629-d3cdd5b7-bab8-4c8a-9d06-95bb585b4298.png)
Figure 7. Distribution of taxi trips and the number of trips of each taxi company in March, June and September.
Each scattered plot is brushable. When we selected a specific area from the scattered plot, the value of bar char will be changed. From those interactive visualizations, selecting the areas with lower fares and higher tips can estimate the company has better service is Top Cab Affiliation in Figure 8.  
![image](https://user-images.githubusercontent.com/80800544/204972643-400ce0b1-0488-4a41-8d51-e10411b3e7e3.png)
Figure 8. Distribution of company with lower fare and higher tips in March, June and September.
Finally, we created three multiple-linked views with timelines and fare in March, June, and September. The plot on the top represents the trips in different months with the trip's start timestamp and fare as the x-axis and y-axis. The plot at the bottom can be selected with a brush. The value of the plot at the top will be changed by either zooming the plot or brushing on the plot at the bottom in Figures 9, 10, and 11.  
![image](https://user-images.githubusercontent.com/80800544/204972676-7e9021a6-ecb7-40fe-99e1-e1a78d784040.png)
Figure 9. Distribution of taxi trips in March based on fare and timeline. 
Finally, we created three multiple-linked views with timelines and fare in March, June, and September. The plot on the top represents the trips in different months with the trip's start timestamp and fare as the x-axis and y-axis. The plot at the bottom can be selected with a brush. The value of the plot at the top will be changed by either zooming the plot or brushing on the plot at the bottom in Figures 9, 10, and 11.  Figure 9. Distribution of taxi trips in March based on fare and timeline. 
![image](https://user-images.githubusercontent.com/80800544/204972692-bac25c5c-eb75-4957-84f1-5c53228493ef.png)
Figure 10. Distribution of taxi trips in June based on fare and timeline.
Finally, we created three multiple-linked views with timelines and fare in March, June, and September. The plot on the top represents the trips in different months with the trip's start timestamp and fare as the x-axis and y-axis. The plot at the bottom can be selected with a brush. The value of the plot at the top will be changed by either zooming the plot or brushing on the plot at the bottom in Figures 9, 10, and 11.  Figure 9. Distribution of taxi trips in March based on fare and timeline. 
![image](https://user-images.githubusercontent.com/80800544/204972709-1c46f081-a379-48ad-bcd5-c37ea3c211b3.png)
Figure 11. Distribution of taxi trips in September based on fare and timeline.
Finally, we created three multiple-linked views with timelines and fare in March, June, and September. The plot on the top represents the trips in different months with the trip's start timestamp and fare as the x-axis and y-axis. The plot at the bottom can be selected with a brush. The value of the plot at the top will be changed by either zooming the plot or brushing on the plot at the bottom in Figures 9, 10, and 11.  Figure 9. Distribution of taxi trips in March based on fare and timeline. 
Comparing the distribution of taxi trips based on fare and timeline in March with the distribution in June and September, we can see the trip with the highest fare in March, June, and September happened on March 24th at 03:15 PM, June 13th at 01:00 PM and September 28th, 02:45 PM in Figure 12, 13, 14.
![image](https://user-images.githubusercontent.com/80800544/204972725-e7bb57d6-ccd9-44eb-a877-3c9cab5d3d8d.png)
Figure 12. Visualization of zooming trips data with the highest fare in March.
![image](https://user-images.githubusercontent.com/80800544/204972739-62d5819b-fdee-4848-ac2d-daec159fde5a.png)
Figure 13. Visualization of zooming trips data with the highest fare in June.
![image](https://user-images.githubusercontent.com/80800544/204972763-95e12355-09c8-4922-8509-dfc5b20dc670.png)
Figure 14. Visualization of zooming trips data with the highest fare in September. 
Based on the data visualization and analysis, we can conclude that Taxicab Insurance Agency, LLC is the most favorable company based on fare distribution because most trips from that company had longer distance and lower fare. Most trips happened in downtown loop and lakeshore areas because there are many views and shopping points there, which attritive more pedestrians. In addition, the taxi company has better service is Top Cab Affiliation. Most trips cost the most happened in the afternoon in March, June and September. Besides the data, the good thing we learn from this project is being familiar with creating a webpage and host visualization using HTML and JavaScript. The important part we want to improve is making multiple-linked-views visualization via spatial map. 

