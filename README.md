# Belly Button Biodiversity Dashboard
This project involved building an interactive dashboard to explore the Belly Button Biodiversity dataset, which catalogued the microbes colonizing human navels. The dataset revealed that a small handful of microbial species (also called operational taxonomic units, or OTUs) were present in more than 70% of people, while the rest were relatively rare.

The Visualisatons are published on the website : https://sindhujasirigeri.github.io/belly_button_challenge/

## Background

In this assignment, the primary objective was to create a dynamic and interactive dashboard to visualize the diversity of microbes found in human belly buttons. The dashboard was designed to include visualizations such as bar charts, bubble charts, and demographic information panels that updated based on user input.

## Project Steps

### Initial Setup
1.  **Repository Creation:**
    -   A new repository named `belly-button-challenge` was created.
    -   The repository was cloned to the local machine.

2.  **File Setup:**
   -   Files from the `StarterCode` folder provided in the Module 14 Challenge zip file were copied into the local git repository. These included `index.html`, `samples.json`, and the `static` folder.

3.  **Deployment Preparation:**
   -   Changes were pushed to GitHub.
    -   The repository was deployed to GitHub Pages.

### Data Visualization
The following steps were completed to build the interactive visualizations:

1.  **Data Loading:**
 -   The D3 library was used to read in `samples.json` from the URL: `https://static.bc-edx.com/data/dla-1-2/m14/lms/starter/samples.json`.

2.  **Bar Chart:**
-   A horizontal bar chart was created with a dropdown menu to display the top 10 OTUs found in an individual.
    -   `sample_values` were used as the values for the bar chart.
    -   `otu_ids` were used as the labels for the bar chart.
    -   `otu_labels` were used as the hovertext for the chart.

3.  **Bubble Chart:**
    -   A bubble chart was created to display each sample.
    -   `otu_ids` were used for the x values.
    -   `sample_values` were used for the y values.
    -   `sample_values` were used for the marker size.
    -   `otu_ids` were used for the marker colors.
    -   `otu_labels` were used for the text values.

4.  **Metadata Display:**
-   The sample's metadata, i.e., an individual's demographic information, was displayed.
    -   Each key-value pair from the metadata JSON object was looped through, and a text string was created.
    -   An HTML tag with that text was appended to the `#sample-metadata` panel.

5.  **Interactive Updates:**
-   All plots were updated when a new sample was selected.

## Skills Acquired
During the development of this project, the following skills were acquired and practiced:

1.  **Data Fetching with D3.js:** Learned how to fetch and parse JSON data from a remote URL using D3.js.
2.  **Data Manipulation:** Gained experience in filtering and processing JSON data to extract relevant information for visualization.
3.  **Dynamic DOM Manipulation:** Utilized D3.js to dynamically update HTML content based on user interactions.
4.  **Interactive Data Visualization with Plotly.js:** Created interactive charts (bar and bubble charts) using Plotly.js and customized their appearance and behavior.
5.  **Event Handling:** Implemented event listeners to handle user interactions and update visualizations accordingly.


## References
Hulcr, J. et al. (2012) A Jungle in There: Bacteria in Belly Buttons are Highly Diverse, but Predictable. Retrieved from: http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/Links to an external site.
