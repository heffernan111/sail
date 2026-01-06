# SailGP Data Analyst Challenge

## Questions Completed

I completed the following questions from the challenge:

1. **Question 1**: Calculate an accurate mean value for a compass direction (e.g., TWD or Heading) across a downsampled frequency.
   - Implemented circular statistics to handle the 0-360° wrap-around problem
   - Created visualizations comparing original vs downsampled data using Bokeh

2. **Question 2**: Calculate a VMC column for a timeseries of boat Lat/Lon values using a course XML.
   - Calculated VMC (Velocity Made Good to Course) for each boat position
   - **Additional features I added**:
     - Tack detection with persistence filtering (to avoid false positives from noise)
     - Gust and lull detection (wind speed increases/decreases)
     - Lift and header detection (favorable/unfavorable wind direction shifts)
     - Multi-panel visualization showing VMC, wind speed with gusts/lulls, and wind direction with lifts/headers

4. **Question 4**: Calculate a Distance to Leader metric for each boat using a timeseries of Lat/Lon positions and a course XML.
   - Calculated distance to the leading boat at each timestamp
   - Visualized distance to leader over time for all boats using Bokeh

## AI Assistance

I used AI tools  to help with this project in the following ways:
- **Initial code polishing**: After writing my initial implementation, I used AI to help polish and refine the code structure
- **Final code cleanup**: Used AI to clean up the final code, improve comments, and ensure consistency across the notebook

## Usage
- The notebook `main.ipynb` contains the code and analysis for the completed questions.
- Each section of the notebook corresponds to a specific question and includes the necessary code, comments, and visualizations.
- All visualizations use Bokeh as requested.