
  
# Weather Dashboard ☁️

## Overview
This project consists of a Python script that extracts weather data from the Open Weather API. This will grab the data from OpenWeather API to ouput it to the S3 bucket and display weather information. 

## Prerequisites
- Python 3.x installed on your machine.
- An OpenWeather API key. You can get one by signing up at [OpenWeather](https://home.openweathermap.org/users/sign_up).
- AWS CLI installed and configured with an IAM user, you can download the AWS CLI from [here](https://aws.amazon.com/cli/).
  
  
## Features

- 🌍 Fetch live weather details for various cities
- 🌡️ Display temperature (°F), 💧 humidity, and 🌈 conditions
- 🗂️ Auto-save weather data in AWS S3 for safekeeping
- 🏙️ Track multiple cities simultaneously
- ⏰ Timestamp data for easy historical analysis


## Project Structure
- `weather_dashboard.py`: The main script that contains the `WeatherDashboard` class. This script fetches weather data from the OpenWeather API, saves the data to an AWS S3 bucket, This script also includes a plot_forecast method that uses Matplotlib to plot the temperature forecast for the next 5 days. The main function has been updated to fetch and plot the forecast for each city. When you run the script, it will display the forecast plots directly.
- [requirements.txt](http://_vscodecontentref_/1): A file that lists all the Python packages required to run the project. These packages can be installed using `pip install -r requirements.txt`.
- [.env](http://_vscodecontentref_/2): A file that contains environment variables such as the OpenWeather API key and AWS bucket name. This file is loaded by the `dotenv` package to configure the application.
- [images](http://_vscodecontentref_/3): A directory to store images used in the [README.md](http://_vscodecontentref_/3) file or other documentation.

## Setup
1. Clone the repository to your local machine.
   ```
    git clone https://github.com/GfavourBraimah/Weather_API_Dashboard
   ```

2. . Create a virtual environment and activate it:
    ```bash
    python -m venv .venv
    source .venv/Scripts/activate  # On Windows
    ```
3. Install the required packages:
   ```
    pip install -r requirements.txt
    pip install matplotlib
    
4. Create a `.env` file in the root directory and add your OpenWeather API key and AWS bucket name:
    ```
    OPENWEATHER_API_KEY=your_openweather_api_key
    AWS_BUCKET_NAME=your_aws_bucket_name

## Usage
1. Run the `weather_dashboard.py` script to fetch weather data:
    ```
    python src/weather_dashboard.py

     ![installation](/images/dashboard.png)
     
## Example
The weather dashboard displays the following information for each city:
- City name
- Temperature (°F)
- Feels like temperature (°F)
- Humidity (%)
- Weather conditions

## Screenshot
![Bucket weather dashboard](/images/weather_bucket.png)   
![Harare_forecast](/images/Harare_forecast.png)       


 ---

## Conclusion

Through this project, I gained hands-on experience with creating and managing AWS S3 buckets, securely handling API keys using environment variables, and applying Python best practices for integrating APIs. I also improved my understanding of Git workflows for efficient project development, learned robust error-handling techniques for distributed systems, and enhanced my skills in managing cloud resources effectively.

