<center>

# Miniproject 1

</center>

## Introduction

<justify>
In this project I was assigned to create a model that will predict the fuel consumption of a cruise ship base on data from several sensors. Data were provided in CSV files of raw sensor outputs. Units of fuel consumption are left open. 

</justify>

## Data preprocessing
<justify>

Each CSV file contains two columns: time and value. Time is in .NET DateTime.Ticks format and needs to be converted to human readable format in order to properly aggregate the data from all sensors.

### Defining the taarget variable

To determine the optimal time window to predict the fuel consumption, I aggregated records by day and counted the number of records. That gave me 54 days with records from all sensors. With minimul number of records per day for one sensor was 5894. I chose the window for predicting the consumption to be 1 hour.

### Feature selection

</justify>
