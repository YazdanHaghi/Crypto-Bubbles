# Crypto-Bubbles

**Crypto Bubbles**

This code visualizes cryptocurrency data using D3.js, focusing on 24h change. The data is displayed in a dynamic circle pack layout, with circles representing cryptocurrencies and their sizes proportional to the chosen variable.

**Features:**

* **Interactive Data Exploration:** Users can update the data displayed in the circles based on market capitalization, volume, price, or circulating supply.
* **Informative Tooltips:** Hovering over a circle reveals additional cryptocurrency information.
* **Clear and Customizable Visualization:** The code is well-structured and documented, allowing for easy customization of the visual style (through CSS) and data (through the `data.json` file).

**Requirements:**

* D3.js library (https://d3js.org/)
* Data file in JSON format (data.json)

**Getting Started:**

1. Save the code as an HTML file (e.g., `crypto_bubbles.html`).
2. Ensure you have D3.js included in your HTML file: `<script src="https://d3js.org/d3.v5.js"></script>`
3. Place your data file (`data.json`) in the same directory as the HTML file.

**How to Use:**

The visualization will load automatically upon opening the HTML file. Click on the radio buttons (currently commented out) to select the desired category (market cap, volume or price) and update the displayed data.(I add just the 24h changes for now).

**Code Structure:**

The code consists of HTML, and JavaScript sections:

* **HTML:** Defines the basic structure of the webpage, including the title and a container for the visualization.
* **JavaScript:**
    * Data processing functions:
        * `millionsFormat`: Formats numbers to millions with commas for market capitalization and volume.
        * `supplyFormat`: Formats supply values with appropriate unit (e.g., Billion).
    * Pack layout creation:
        * `pack`: Creates a D3 pack layout with specific settings.
    * Data loading and processing:
        * Loads data from `data.json` and formats it for consistency.
        * Creates a hierarchy from the data for the pack layout.
    * Visualization creation:
        * Defines tooltips and their behavior on hover.
        * Creates SVG elements and sets their dimensions.
        * Uses the pack layout to position circles within the SVG.
        * Appends circles, labels, and text elements to represent the data points.
    * Update function:(is commented in the project but the function is working just uncomment the html code to use it)
        * `updateData`: Allows users to change the variable used to size the circles and updates the visualization accordingly.

**Further Customization:**

* Edit the `data.json` file to include your desired cryptocurrency data structure. Ensuring consistent formatting (e.g., comma separators for numbers) is crucial for proper data processing.
* Explore D3.js documentation (https://d3js.org/) to customize the visualization further, such as adding animations or interactions.

!["Alt text for your image"](["(https://github.com/YazdanHaghi/Crypto-Bubbles/blob/main/Screenshot%202024-06-04%20193450.png)"])

