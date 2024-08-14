**Inventory Management Dashboard**

**Overview**

This repository contains a Dash-based web application designed to manage and visualize product inventory across various locations. 
The application allows users to filter products based on location and set quantity thresholds to identify products that fall below a certain inventory level.

**Features**

    Location Filter: Users can select a location from a dropdown menu where the options are a combination of location ID and name.
    Quantity Threshold: A numeric input field allows users to set a threshold for the minimum quantity of products.
    Dynamic Data Table: The app displays a filtered list of products that fall below the set threshold for the selected location.

**Prerequisites**

Ensure you have the following Python libraries installed:

    dash
    dash-bootstrap-components
    pandas

**Code Structure**

    app.py: The main application script that initializes the Dash app, defines the layout, and implements the callback functions to update the data table based on user inputs.

**Application Components**

    Header: Displays the title of the dashboard.
    Filters:
        Location Dropdown: Filters data based on selected location (loc_id and loc_nam concatenated).
        Quantity Threshold Input: Sets a threshold to filter products below a certain quantity.
    Data Table: Displays the filtered list of products with selected attributes such as prod_name, prod_attribute, prod_thc_lvl, etc.

**Callback Function**

The callback function updates the data table based on the selected location and quantity threshold:

    Input: Location and quantity threshold.
    Output: A data table filtered to show only relevant products.

**License**

This project is licensed under the MIT License
