# SailGP Data Analyst Challenge

## Overview

This project is aimed at analyzing the data from the SailGP event in Auckland 2025. The data is provided in various formats and the goal is to answer specific questions using Python. The analysis includes data processing, visualization, and deriving insights from the provided datasets.

## Data Sources

- **Boat Logs**: Located in the `Boat_Logs` folder. The data is in CSV format and the columns are described in the `Boat_Logs/Boat_Logs_Columns.csv` file.
- **Course Marks**: The `Course_Marks_2025-01-19.csv` file contains the mark positions and wind readings on the course for the whole day.
- **Race XML**: The `Race_XML` folder contains XML files for each race that include information on course boundaries, theoretical mark positions, and target racecourse axis.
- **Manoeuvre Summary**: The `2025-01-19_man_summary.csv` file contains metrics from the manoeuvre summary for the day.
- **Straight Line Summary**: The `2025-01-19_straight_lines.csv` file contains metrics from the straight line summary for the day.
- **Polar Data**: The `2502 m8_APW_HSB2_HSRW.kph.csv` file contains the polar data for the boats in that configuration.

## Requirements

- Python 3.8 or higher
- Jupyter Notebook
- Suggested Libraries: `pandas`, `numpy`, `bokeh`, `beautifulsoup4`(to read xmls), `matplotlib`, `scipy`

## Setup

1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Install the required libraries:
    ```sh
    pip install pandas numpy bokeh matplotlib scipy etc....
    ```

3. Open the Jupyter Notebook:
    ```sh
    jupyter notebook main.ipynb
    ```

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


8. **Question 8**: Provide insights on what made a team win or underperform in the race.
   - Analyzed race results, tack counts, and VMG metrics
   - Compared winners vs other boats to identify key performance factors
   - Created visualizations showing the relationship between tacks, VMG, and race position
   - Provided evidence-based insights on minimum tacks and maximum VMG strategies

## AI Assistance

I used AI tools (specifically Cursor's AI assistant) to help with this project in the following ways:
- **Initial code polishing**: After writing my initial implementation, I used AI to help polish and refine the code structure
- **Final code cleanup**: Used AI to clean up the final code, improve comments, and ensure consistency across the notebook
- The core logic, analysis approach, and visualizations were all my own work

## Usage
- The notebook `main.ipynb` contains the code and analysis for the completed questions.
- Each section of the notebook corresponds to a specific question and includes the necessary code, comments, and visualizations.
- All visualizations use Bokeh as requested.


## Contact

For any questions or inquiries, please contact [drey@sailgp.com], [kkonig@sailgp.com].