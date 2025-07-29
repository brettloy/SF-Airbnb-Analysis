# 🗺️ San Francisco Airbnb Interactive Map

This Tableau project visualizes Airbnb activity across San Francisco neighborhoods using spatial and listing data. The dashboard allows users to explore neighborhood-level metrics like average price per night, listing density, and value score (calculated as average rating per price). The interactive map helps identify which areas are most expensive, most popular, and best value for guests.

---

## 🔍 Key Features
- **Interactive Map** of San Francisco neighborhoods using GeoJSON polygons
- **Color-coded by metric**: average price, listing count, or value score
- **Hover tooltips** show per-neighborhood stats like:
  - Average Price (USD)
  - Average Rating
  - Total Listings
  - Value Score = Avg Rating ÷ Avg Price
- **Filters** for room type, bedroom count, and more
- **Built entirely in Tableau Public**

---
▶️ **View the interactive map:**  
[Click here to open in Tableau Public](https://public.tableau.com/app/profile/brett.loy/viz/Book1_17523558376460/AirbnbTrendsinSanFrancisco?publish=yes&showOnboarding=true)

## 📁 Project Files
| File | Description |
|------|-------------|
| `SF_Map.twbx` | Tableau Packaged Workbook containing the full dashboard |
| `listings_summary.csv` | Pre-processed Airbnb listing data grouped by neighborhood |
| `neighborhoods.geojson` | GeoJSON file with San Francisco neighborhood boundaries |
| `screenshots/` | Optional preview images of the dashboard |
| `README.md` | This documentation file |

---

## 🧰 Tools Used
- **Tableau Public**: Data visualization and dashboard creation
- **GeoJSON**: Spatial boundaries of SF neighborhoods
- **CSV**: Airbnb listing data from [InsideAirbnb](http://insideairbnb.com/get-the-data.html)
- **GitHub**: Version control and public documentation

---

## 🗃️ Data Sources
- **Airbnb Listings (August 2023)**:  
  Downloaded from [InsideAirbnb – San Francisco](http://insideairbnb.com/get-the-data.html)  
  Contains fields like `price`, `review_scores_rating`, `neighbourhood`, `room_type`, and `number_of_reviews`.

- **Neighborhood GeoJSON**:  
  [SF Planning Department / DataSF](https://data.sfgov.org) – "SF Find Neighborhoods" shapefile or GeoJSON.

---

## 🧠 How It Works
1. **Cleaned the Airbnb data** using SQL to remove `$`, convert data types, and group by neighborhood.
2. **Joined** the summary table to the SF GeoJSON in Tableau using the `neighborhood` field.
3. Built an **interactive choropleth map** in Tableau with custom tooltips, color scales, and filters.
4. **Published** the final visualization to Tableau Public and linked it here on GitHub.

---

## 📌 Use Cases
- Market analysis for hosts or property investors
- Academic or data science portfolio project
- Tourism trend exploration
- Interactive storytelling using geospatial data


