# 30 Days DevOps Challenge - Weather Dashboard

Day 1: Building a weather data collection system using AWS S3 and OpenWeather API

# Weather Data Collection System - DevOps Day 1 Challenge

## Project Overview
This project is a Weather Data Collection System that demonstrates core DevOps principles by combining:
- External API Integration (OpenWeather API)
- Cloud Storage (AWS S3)
- Infrastructure as Code
- Version Control (Git)
- Python Development
- Error Handling
- Environment Management

## Features
- Fetches real-time weather data for multiple cities
- Displays temperature (°F), humidity, and weather conditions
- Automatically stores weather data in AWS S3
- Supports multiple cities tracking
- Timestamps all data for historical tracking

## Technical Architecture
- **Language:** Python 3.x
- **Cloud Provider:** AWS (S3)
- **External API:** OpenWeather API
- **Dependencies:** 
  - boto3 (AWS SDK)
  - python-dotenv
  - requests

## Manual Tasks 
<ul>
  <li>Sign-Up for OpenWeather API</li>
  <li>configure env variables</li>
  <li> create s3 bucket via CLI instead of weather_dashboard.py script
    <ul> 
      <li> s3 bucket command: </li>  
      `aws s3 mb s3://day1-weatherdashboard --region us-east-1`
      
  ![create_s3_bucket](https://github.com/user-attachments/assets/bef90e42-b789-4b02-8e58-035de9a5ed18)       
    </ul>
  </li>
</ul>

## Day-1 Project Reaction
<p> Major shoutout and appreciation to Alicia Ahl, DeShae Lyda, Ifeanyi Otuonye, and Kathryn Jones. Day 1 weather dashboard was fun. Great way to start the challenge. I beleive I will learn a lot and enhance my DevOps skillset.</p>  

Script Output:

![script_output](https://github.com/user-attachments/assets/fb34be15-53e1-4751-b6a5-a02bd5f381ce)

![s3_bucket](https://github.com/user-attachments/assets/1ea62e9e-050e-4249-911b-fb9ce83ae322)

```markdown
## Project Structure
weather-dashboard/
  src/
    __init__.py
    weather_dashboard.py
  tests/
  data/
  .env
  .gitignore
  requirements.txt

## Setup Instructions
1. Clone the repository:
--bash
git clone https://github.com/ShaeInTheCloud/30days-weather-dashboard.git

3. Install dependencies:
bashCopypip install -r requirements.txt

4. Configure environment variables (.env):
CopyOPENWEATHER_API_KEY=your_api_key
AWS_BUCKET_NAME=your_bucket_name

4.Configure AWS credentials:
bashCopyaws configure

5. Run the application:
python src/weather_dashboard.py

What I Learned

AWS S3 bucket creation and management
Environment variable management for secure API keys
Python best practices for API integration
Git workflow for project development
Error handling in distributed systems
Cloud resource management

Future Enhancements

Add weather forecasting
Implement data visualization
Add more cities
Create automated testing
Set up CI/CD pipeline


