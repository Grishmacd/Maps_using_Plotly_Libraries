# Maps_using_Plotly_Libraries

This code demonstrates two types of **interactive geographic visualizations** using Plotly Express:
1. A **choropleth map** to color countries based on a numeric value
2. A **scatter geo map** to plot cities using latitude/longitude with bubble sizes

---

## What this visualization shows

### 1) Choropleth Map (Country-wise Values)
- Colors each country based on a numeric `value`
- Useful for comparing metrics across countries (example: score, index, rate)
- Uses a continuous color scale (**Viridis**) for clear variation

**Key mapping used:**
- `locations="country"`
- `locationmode="country names"`
- `color="value"`

---

### 2) Scatter Geo Map (Cities around the World)
- Plots cities using `lat` and `lon`
- Bubble size represents `population`
- Hover shows the city name

**Key mapping used:**
- `lat="lat"`, `lon="lon"`
- `size="population"`
- `hover_name="city"`
- `projection="natural earth"`

---

## Data Used

### Choropleth Data
- Countries: India, United States, China, Brazil, Russia
- Values: 90, 75, 88, 65, 70

### Scatter Geo Data
- Cities: Delhi, New York, Tokyo, London
- Latitude/Longitude provided for each city
- Population used to scale bubble size

---

## Libraries Used
- `plotly.express`  
  Used to generate interactive maps:
  - `px.choropleth()`
  - `px.scatter_geo()`
- `pandas`  
  Used to create DataFrames for map inputs.

---

## Output
- An interactive choropleth titled: **"Sample Choropleth Map (Country-wise Values)"**
- An interactive scatter geo map titled: **"Scatter Geo Map (Cities around the World)"**

---

## Developer
Grishma C.D
