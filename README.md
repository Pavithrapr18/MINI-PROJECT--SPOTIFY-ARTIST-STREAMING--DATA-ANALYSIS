🎵 Spotify Artist Streaming Analytics

📌 Project Overview

Spotify Artist Streaming Analytics is a data analytics and visualization project developed to explore Spotify music data and identify meaningful patterns in artist performance, track popularity, streaming activity, release trends, genres, and audio characteristics.

The project uses Microsoft Excel for data cleaning and preprocessing and Microsoft Power BI for data analysis and interactive dashboard development.

The final dashboard provides a visual and user-friendly way to explore music-related data through KPI cards, charts, maps, and analytical visualizations.

🎯 Objectives

The main objectives of this project are:

Analyze Spotify track and artist data.
Identify the most streamed artists and tracks.
Analyze streaming performance across different genres.
Examine track popularity and streaming counts.
Study music release patterns across years, months, quarters, and days.
Analyze audio characteristics such as danceability, energy, tempo, loudness, and instrumentalness.
Explore relationships between popularity and audio features.
Compare explicit and non-explicit tracks.
Analyze streaming activity across different countries.
Develop an interactive and visually appealing Power BI dashboard.
Present complex music data in an easy-to-understand format.

📊 Dataset

The dataset used for this project is:

Spotify Artist Streaming Analytics 2020–2025

Source: Kaggle

The dataset contains information about Spotify tracks, artists, albums, genres, release dates, streaming counts, popularity, and audio features.

Main Attributes
Category	Attributes
Track Information	Track ID, Track Name, Album Name
Artist Information	Artist Name, Artist Track Count
Release Information	Release Date, Release Year, Release Month, Release Day of Week, Release Quarter
Genre	Genre
Streaming	Stream Count
Popularity	Popularity
Audio Features	Danceability, Energy, Tempo, Loudness, Instrumentalness
Music Properties	Key, Key Name, Mode, Mode Name
Content	Explicit, Is Explicit
Geographic	Country
Other	Label, Duration Minutes, Is Weekend Release

🧹 Data Cleaning and Preprocessing

The raw dataset was first processed using Microsoft Excel before being imported into Power BI.

Cleaning Steps
Reviewed the structure of the dataset.
Selected the required number of records for the project.
Removed unnecessary and duplicate columns.
Checked for missing values.
Corrected data types.
Standardized text values.
Verified artist and track names.
Checked release-date formatting.
Created/validated release year and month information.
Checked release quarter and weekday information.
Verified numerical values such as:
Popularity
Danceability
Energy
Tempo
Loudness
Stream Count
Removed duplicate versions of fields where appropriate.
Prepared the cleaned dataset for Power BI.

🔄 Project Workflow
        Raw Spotify Dataset
                ↓
       Data Cleaning in Excel
                ↓
        Data Validation
                ↓
       Data Transformation
                ↓
          Clean Dataset
                ↓
        Import into Power BI
                ↓
         Data Modeling
                ↓
        DAX Calculations
                ↓
       Dashboard Development
                ↓
       Data Visualization
                ↓
      Analysis & Interpretation
      
📊 Power BI Dashboard

The Power BI dashboard is organized into three major pages.

🏠 Page 1 — Spotify Overview

The first page provides an overall summary of Spotify streaming activity.

KPI Cards
Total Tracks
Total Artists
Total Streams
Average Popularity
Average Energy
Visualizations

🎤 Top 10 Artists by Stream Count

A horizontal bar chart showing the artists with the highest total stream counts.

🎵 Top 10 Tracks by Stream Count

Displays the tracks with the highest streaming activity.

🔞 Explicit vs Non-Explicit Tracks

A donut chart comparing explicit and non-explicit tracks.

🎼 Streams by Genre

Shows total streaming activity across different music genres.

🌍 Streams by Country

A geographic visualization showing the distribution of streams across countries.

Purpose

This page provides a quick overview of:

Artist performance
Track performance
Streaming activity
Genre popularity
Geographic distribution
Explicit content distribution

📅 Page 2 — Release Analysis

The second page focuses on music release patterns.

Visualizations

📈 Tracks Released by Year

Chart: Line chart

X-axis → Release Year
Y-axis → Count of Track ID

Shows how the number of releases changes over the years.

📊 Tracks Released by Month

Chart: Column chart

X-axis → Release Month
Y-axis → Count of Track ID

Shows which months have more releases.

📊 Tracks Released by Quarter

Chart: Column chart

X-axis → Release Quarter
Y-axis → Count of Track ID

Compares Q1, Q2, Q3, and Q4.

📊 Tracks Released by Day of Week

Chart: Column chart

X-axis → Release Day of Week
Y-axis → Count of Track ID

Shows release activity by day.

🍩 Weekend vs Weekday Releases

Chart: Donut chart

Legend → Is Weekend Release
Values → Count of Track ID

Compares weekend and weekday releases.

📈 Release Trends by Genre

Chart: Line chart

X-axis → Release Year
Y-axis → Count of Track ID
Legend → Genre

Shows how release activity for different genres changes over time.

Purpose

This page helps understand:

Yearly release patterns
Monthly release patterns
Quarterly trends
Preferred release days
Weekend vs weekday releases
Genre-specific release trends

🎧 Page 3 — Audio Analysis

The third page focuses on the audio characteristics of Spotify tracks.

KPI Cards
Average Popularity
Average Danceability
Average Energy
Average Tempo
Visualizations

💃 Average Danceability by Genre

Compares average danceability across genres.

⚡ Average Energy by Genre

Compares average energy across different genres.

📈 Popularity vs Danceability

Chart: Scatter plot

X-axis → Danceability
Y-axis → Popularity

Used to explore the relationship between danceability and popularity.

📈 Popularity vs Energy

Chart: Scatter plot

X-axis → Energy
Y-axis → Popularity

Used to explore the relationship between energy and popularity.

🎵 Average Tempo by Genre

Compares average BPM across genres.

🎹 Average Instrumentalness by Genre

Compares instrumentalness levels across genres.

🔊 Average Loudness by Genre

Compares average loudness across genres.

Purpose

This page helps analyze:

Audio characteristics by genre
Popularity relationships
Danceability
Energy
Tempo
Instrumentalness
Loudness

🧮 DAX Measures

Several DAX measures can be used to support the dashboard.

Total Streams =
SUM('Spotify'[Stream Count])
Total Tracks =
DISTINCTCOUNT('Spotify'[Track ID])
Total Artists =
DISTINCTCOUNT('Spotify'[Artist Name])
Average Popularity =
AVERAGE('Spotify'[Popularity])
Average Energy =
AVERAGE('Spotify'[Energy])
Average Danceability =
AVERAGE('Spotify'[Danceability])
Average Tempo =
AVERAGE('Spotify'[Tempo])
🛠️ Technologies Used
Microsoft Excel

Used for:

Data cleaning
Data preprocessing
Data validation
Formatting
Removing unnecessary data
Preparing the dataset
Microsoft Power BI

Used for:

Data visualization
Dashboard development
KPI cards
Charts
Maps
Interactive analysis
Data modeling
DAX

Used for:

Calculated measures
Aggregations
KPI calculations
Analytical metrics

🎨 Dashboard Design

The dashboard follows a Spotify-inspired theme.

Design Elements
Dark green
Spotify green
Black
White
Light green
Rounded cards
Music-themed imagery
Consistent typography
Green-colored charts
Clean navigation sidebar

The navigation contains:

🏠 Overview

📊 Release Analysis

🎧 Audio Analysis

The active page is highlighted using a green accent.

📈 Key Analytical Areas

The project focuses on several major analytical areas:

Artist Analysis

Identifies artists with high streaming activity.

Track Analysis

Identifies highly streamed tracks.

Genre Analysis

Compares streaming and audio characteristics across genres.

Release Analysis

Studies when music is released.

Audio Analysis

Examines the characteristics of music tracks.

Geographic Analysis

Explores streaming activity across countries

📁 Project Structure

Spotify-Artist-Streaming-Analytics/
│
├── Dataset/
│   └── spotify_cleaned.xlsx
│
├── PowerBI/
│   └── spotify_artist_streaming_analytics.pbix
│
├── Documentation/
│   └── Project_Report.pdf
│
└── README.md

🔐 Data Considerations

The project is intended for educational and analytical purposes.

The dashboard represents patterns in the provided dataset and should not be interpreted as an official representation of Spotify's complete global streaming data.

🚀 Future Enhancements

The project could be extended with:

Real-time Spotify API integration
More recent streaming data
Advanced artist segmentation
Machine learning-based popularity prediction
Time-series forecasting
Recommendation analysis
Sentiment analysis of song lyrics
Interactive drill-through pages
Automated dashboard refresh
More detailed geographic analysis

📌 Conclusion

Spotify Artist Streaming Analytics demonstrates how raw music data can be transformed into meaningful insights using Excel, Power BI, and DAX.

The project combines data preprocessing, analytical calculations, and interactive visualizations to examine artist performance, track streaming, genres, release patterns, geographic distribution, and audio characteristics.

The final Power BI dashboard provides a clear and visually engaging platform for exploring Spotify-related data and demonstrates practical skills in data cleaning, data analysis, visualization, dashboard design, and business intelligence.

👩‍💻 Project Information

Project Title: Spotify Artist Streaming Analytics
Project Type: Data Analytics & Visualization Mini Project
Domain: Music Analytics
Tools: Microsoft Excel, Microsoft Power BI, DAX
Dataset Source: Kaggle
Dashboard Pages: 3
Primary Output: Interactive Power BI Dashboard
