 # **Covid-19 cases Across countries in Africa.**

## **Discription**

This repository contains python code that analyses covid-19 cases across countries in Africa. I got the data from https://www.kaggle.com/datasets/okwirjulius/covid19-cases-in-africa?, which is in csv format. I checked for columns with null values and missing values were detected in two countries.  At the time of data collation, there were no records for missing values in 'Comoros' and 'Tanzania', ttherefore I replaced the missing values with zero using a function from pandas’ library. The original dataset does not contain country iso alpha code, I had to add iso alpha code to each country in order to be able to locate each country precisely on the map. The visualization was achieved by using choropleth heatmap from Plotly Express and the final result is displayed using Dash framework. I limit my scope to Africa heatmap because, the project is concerned about Africa. The visualization contains four (4) radio buttons namely “Total Cases”, “Total Deaths”, “Total Recovered”, and “Active Cases” respectively(as shown in the figure below). Each radio button gives different visualization when clicked, which enable the user to get the information needed easily and faster.
![screen](https://github.com/Piemicah/covid/assets/93428049/34f86128-5b39-4951-96eb-2e4464fa4bc2)

I also generated horizontal bar visualization for the total cases using Plotly Express bar plot.
![bar](https://github.com/Piemicah/covid/assets/93428049/f245425e-0c6f-4b40-b554-cc186c314cfb)

## **Key User Group**
Regional director (RD) of World Health Organization (WHO) , Africa branch. The role of regional director is to enhance Africa’s technical support to countries for scaling up proven public health interventions.

## **Problem The Regional Director Faces**
Going through a lot of records to know the exact number of people in each country that need urgent medical attentions during the outbreak and the amount of vaccines to be delivered to each country.

## **My Solution**
With my method of visualization and the features(columns) I selected, it becomes so easy for the regional director to know the exact number of active cases, total recovered cases, total deaths and total cases of Covid-19 . He can easily navigate through the visualization and extract the information needed.

## **User Objectives**
* To know the exact number of total cases of covid-19 across countries in Africa. 
*	To know the exact number of  total deaths caused by Covid-19 in each country.
*	To know the exact number of active cases across countries in Africa.
*	To know the exact number of people that have recovered.
*	To be able to calculate the amount to be spent on the affected countries.

## **Visualization Strategy and how the users can achieve best out of it**
Four radio buttons are provided in the visualization that represent four different important features(columns) of the dataset namely “Total Cases”, “Total Deaths”, “Total Recovered”, and “Active Cases”. The radio buttons are created using Dash Core Component (dcc). When each radio button is selected, it gives the visualization corresponding to the label on it e.g if “Total Deaths” is clicked ,it displays total deaths across the heatmap of Africa. User can zoom-in or zoom-out to any scale. User can also hover over each country and a tooltip showing the information of the country is displayed.

## **Additional Features**
1.	Box select: user can drag a box across a specific area of the visualization to have a better view of the selected area.
2.	Pan: user can move the whole map by holding down the left button of the mouse in other to see the hiding part of the map
3.	Hover: User can hover the mouse over the map to get the information about the country under the mouse.

## **How to use**
1.	Clone the repository
2.	Install the requirements
3.	Run the code in GitHub using codespaces
4.	Explore and navigate through the visualization as you wish
