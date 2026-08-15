# Music Trends & Artist Insights Dashboard

An interactive Power BI dashboard built on Spotify's Top 50 global 
songs dataset, exploring what drives song popularity across artists, 
release dates, and album types.

## Data Model
- Core table: Top-50-world (song, artist, popularity, release_date, 
  album_type, album_cover_url)
- Custom DAX measures: Average Popularity, Average Duration (min), 
  Artist Top Song (dynamic TOPN measure returning each artist's 
  highest-ranked track)

## Pages
1. **Home** — Landing/navigation page
2. **Overview** — KPI cards (distinct songs, average popularity, 
   average duration), popularity trend by month/year, explicit vs. 
   non-explicit song split, album type breakdown, top artists by 
   song count
3. **Artists** — Artist-level drill-through with song-level popularity 
   rankings, release trends by month, and a Song & Artist slicer for 
   interactive filtering

## Key Features
- Dynamic "Top Song" DAX measure that recalculates per artist using 
  TOPN + ALLSELECTED, powering the drill-through page
- Time-based trend analysis using Date Hierarchy (Year/Month) on 
  release dates
- Interactive slicers for song- and artist-level filtering

## Tools
Power BI, DAX, Data Modeling
