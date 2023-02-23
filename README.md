# Scheduling-Time-Analysis



TASK 1:   


Import necessary modules: datetime for working with dates and times, and plotly.graph_objs for creating the heatmap graph.

Define the data: data is a list of dictionaries, with each dictionary containing information about an item that was scheduled. Each dictionary has three key-value pairs: item_date (the date the item is scheduled for), item_name (the name of the item), and scheduled_time (the time the item is scheduled for).

Convert the item_date and scheduled_time strings in the data to datetime objects using datetime.strptime.

Determine the min and max dates in the data using list comprehension.

Create a dictionary called scheduling_data to hold scheduling information for each date. The dictionary has dates as keys and empty dictionaries as values.

Loop through the data and populate scheduling_data with information about the number of items scheduled for each hour of each date.

Create lists for the x and y values of the heatmap. x_values contains the dates, and y_values contains the hours (0-23). The corresponding value for each date/hour combination is stored in z_values.

Create the heatmap using go.Heatmap with x, y, and z as the x-axis, y-axis, and z-axis data, respectively. The colorscale parameter sets the color scheme, and zmin and zmax set the minimum and maximum values for the color scale. The colorbar parameter sets the title for the colorbar.

Create the layout for the graph using go.Layout. The title parameter sets the title, and the xaxis and yaxis parameters set the titles for the x-axis and y-axis, respectively.

Create a Figure object with the heatmap and layout, and the graph is ready to be displayed with fig.show().




TASK 2


Load data from a JSON file using the json module.
Define a date range using datetime objects.
Filter the data based on the selected date range using a list comprehension.
Calculate the number of items scheduled one day and two days prior to their item date.
Calculate the percentages of items scheduled one day and two days prior to their item date.
Create a bar chart using matplotlib.pyplot showing the percentages of items scheduled one day and two days prior to their item date.
The bar chart shows two bars labeled "1 day prior" and "2 days prior" representing the percentage of items scheduled one and two days prior to their item date respectively. The x-axis represents the number of days prior to the item date and the y-axis represents the percentage of scheduling. The chart is titled "Prior Scheduling Time" and has x and y axis labels.




