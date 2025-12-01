# Smart-City-Mobility-Traffic-Flow-Optimisation
The goal of this data-driven analysis of urban mobility patterns is to increase traffic efficiency across developing metropolitan areas. The project's main goals are to model travel behavior, identify congestion hotspots, comprehend peak-hour flow dynamics, and provide city planners with visual solutions for decongestion and mobility optimization.

Purpose:
The objective of this project is to use data-driven insights to analyze urban mobility patterns and optimize traffic flow in a smart city setting. The project creates useful visualizations and predictive tools that assist engineers, policymakers, and urban planners in making well-informed mobility decisions by examining congestion trends, peak-hour behavior, and movement patterns.

Technologies used:
PowerBI
OpenCity Urban Data Portal
CSV/Excel


Setup Instructions:
1. Install Power BI
Ensure you have one of the following installed:
Power BI Desktop (recommended) – free for Windows
Power BI Service (web version) – optional for publishing dashboards

2. Preparing Your Dataset

Your datasets for Smart City Mobility & Traffic Flow should contain at least the following fields:

Traffic Density / Congestion Dataset
Latitude, Longitude
Area / Road Segment Name
Vehicle Count or Congestion Index
Timestamp
Peak vs Off-Peak Movement Dataset
Timestamp (Date + Time)
Traffic Volume
Speed / Travel Time
Road Segment or Zone
Origin–Destination (OD) Flow Dataset
Origin Zone
Destination Zone
Trip Count / Flow Volume
Time or Time Range (optional)
Congestion Prediction Dataset
Timestamp
Predicted Congestion Level
Confidence Score (optional)
Place the files inside your project folder:

data/
    traffic_density.csv
    peak_offpeak.csv
    od_flow.csv
    congestion_predictions.csv


You can store your dataset anywhere on your system — Power BI can connect to CSV/Excel directly.

3. Open the Power BI Report File

Go to your project folder and open your Power BI report, for example:
SmartCity-Traffic-Analysis.pbix
If Power BI prompts you to reconnect the dataset:
Click Transform Data → Data Source Settings
Browse and link your CSV/Excel files again
Power BI will refresh all visuals automatically

4. Set Data Types & Geographic Fields

To make your maps, heatmaps, and OD flows work properly, check the geographic roles:
Set Geographic Data Types
In the Fields pane, right-click Latitude → Data category → Latitude
Right-click Longitude → Data category → Longitude
For Zone / Area / Road Name:
Use Data category: Place, City, Area, or leave as plain text if using custom visuals
Time Columns
Ensure your timestamp column is set to Date/Time
For hour-based visuals, create a column like “Hour of Day”

5. View the Dashboards

Open the dashboards already included in your project:
Smart City Dashboards
Traffic Density Heatmap
Visualizes congestion hotspots across the city.
Peak vs Off-Peak Flow Comparison
Shows movement differences across morning, noon, evening, and night.
Origin–Destination (OD) Flow Diagram
Displays travel demand between major zones or corridors.

Congestion Prediction Dashboard
Provides estimated congestion levels using ML output data.
Each of these dashboards will refresh automatically when you reconnect or update your dataset.

6. (Optional) Enable Mapping Layers

If your maps do not load correctly:
Click Options → Preview features, enable:
Shape Map
ArcGIS Maps (optional)
Restart Power BI

In your map visual:
Choose Background Maps → Default
Enable layers like:
Roads
Labels
Points of Interest

This ensures proper rendering of congestion and OD flow visuals.

7. Chart and Graph Interactions
Power BI allows rich interactions across visuals:
Click zones on the heatmap to filter OD flows
Use time sliders to compare peak/off-peak patterns
Hover on congestion hotspots to see density values
Filter predicted congestion by date/time
Zoom/pan on the maps for deeper exploration

Usage:
1. Load the Dataset

Open the Power BI report file (.pbix)
If Power BI prompts you to reconnect your data:
Go to Transform Data → Data Source Settings
Reconnect your CSV/Excel files (traffic density, OD flows, peak-hour data, predictions)
Power BI will automatically refresh all visuals and dashboards.

2. Explore the Dashboards

Several dashboards have been created to help you analyze mobility, congestion, and traffic patterns across the city.
Traffic Density Heatmap
View real-time or historical traffic density across zones.
Mouse over hotspots to see:
Vehicle count
Congestion index
Timestamp

Use filters to switch between:
Weekday vs weekend
Morning, afternoon, evening, night
Peak vs Off-Peak Movement Analysis

Compare travel patterns during:
Peak hours vs Non-peak hours
Observe movement speed, volume, and variation over time.
Identify time windows that require traffic control or signal optimization.
Origin–Destination (OD) Flow Diagram
Visualize which zones people are traveling from and to.
High-volume corridors appear with thicker lines.

Filter by:
Time of day
Zone
Type of movement (commuter, commercial, etc.)
This helps identify critical mobility corridors and potential bottlenecks.
Congestion Prediction Dashboard
Displays AI/ML-based congestion predictions for upcoming hours.
Hover over prediction nodes to see:
Expected congestion level
Confidence score
Affected road segments
Helps urban planners prevent congestion before it happens.

3. Apply Filters and Interactions

You can interact with dashboards using multiple tools:
Time Range Slider
Adjust to view patterns across specific hours or days.
Zone / Road Segment Filter
Narrow down congestion or OD flows to targeted locations.
Traffic Type / Vehicle Volume Filter
Compare normal flow vs congested flow.
Zoom & Pan on Maps
Explore local-level hotspots or city-wide traffic patterns.
Click to Highlight
Select any zone, corridor, or flow line to isolate related data.
Tooltip Details
Hover on heatmap points, OD flows, and prediction nodes for detailed numeric insights.
These interactions help you focus on areas with the most traffic pressure or emerging congestion.

4. Export Reports

Power BI allows you to export findings for presentations or analysis:
You can export:
PDF files
PNG/JPEG images
Excel summaries
Data tables (crosstab/export)
Power BI Template (.pbit)
Go to File → Export to download your desired format.

5. Refresh With New Data

To update the dashboards with new traffic or mobility datasets:
Replace the old CSV/Excel files with the new ones (same column structure).
Open the Power BI .pbix file.
Click Refresh on the Home Ribbon.
All dashboards (heatmaps, OD flows, peak/off-peak visuals, predictions) will update automatically.



