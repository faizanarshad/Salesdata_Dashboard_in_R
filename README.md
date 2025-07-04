# Sales Data Dashboard in R

A comprehensive data visualization project that combines multiple datasets to create interactive dashboards using R Markdown and Flexdashboard. This project analyzes both suicide data and laptop sales data, providing insights through various interactive visualizations.


*Screenshot of the Suicide Data Analysis Dashboard showing interactive visualizations and modern styling*

## 📊 Project Overview

This project demonstrates advanced data visualization techniques in R, combining two distinct datasets:
- **Suicide Data**: Global suicide statistics from 1985-2015
- **Laptop Sales Data**: Laptop specifications and ratings from various brands

## 🎯 Features

### Interactive Visualizations
- **Pie Charts**: Brand ratings and suicide distribution by sex
- **Scatter Plots**: Suicide trends by age groups and GDP relationships
- **Bar Charts**: Population vs suicide rates, display size distributions, and decade analysis
- **Heatmaps**: Country-wise suicide data visualization by decade
- **Interactive Plots**: Using Plotly and Highcharter libraries
- **Enhanced Styling**: Custom CSS with gradients, animations, and modern design

### Dashboard Components
- **Flexdashboard**: Responsive layout with multiple columns
- **Real-time Data Processing**: Dynamic data manipulation and visualization
- **Color-coded Visualizations**: Using Viridis color palettes
- **Responsive Design**: Adapts to different screen sizes
- **Custom CSS Styling**: Modern gradients, hover effects, and animations

## 📁 Project Structure

```
Salesdata_Dashboard_in_R/
├── README.md                           # This file
├── SucideData.csv                      # Global suicide statistics dataset
├── laptops.csv                         # Laptop specifications and ratings dataset
├── Suicide_Data_Analysis.Rmd           # Comprehensive suicide data analysis dashboard
├── Suicide_Data_Analysis.html          # Compiled HTML version
├── suicide_styles.css                  # Custom CSS styling for suicide dashboard
├── Laptop_Story_Enhanced.Rmd           # Enhanced laptop data analysis dashboard
├── Laptop_Story_Enhanced.html          # Compiled HTML version
├── enhanced_styles.css                 # Custom CSS styling for laptop dashboard
├── Combine_Two_DataSet.html            # Combined dataset dashboard (HTML)
└── Project_Two.html                    # Original suicide analysis (HTML)
```

## 📊 Datasets

### Suicide Data (`SucideData.csv`)
Contains global suicide statistics with the following variables:
- `country`: Country name
- `year`: Year of data (1985-2015)
- `sex`: Gender (male/female)
- `age`: Age group categories
- `suicides_no`: Number of suicides
- `population`: Population count
- `suicides.100k.pop`: Suicide rate per 100,000 population
- `gdp_per_capita`: GDP per capita
- `generation`: Generation classification

### Laptop Data (`laptops.csv`)
Contains laptop specifications and ratings:
- `name`: Laptop model name
- `price(in Rs.)`: Price in Indian Rupees
- `processor`: Processor specifications
- `ram`: RAM capacity
- `os`: Operating system
- `storage`: Storage type and capacity
- `display(in inch)`: Display size
- `rating`: Customer rating
- `no_of_ratings`: Number of ratings
- `no_of_reviews`: Number of reviews

## 🛠️ Installation & Setup

### Prerequisites
- R (version 4.0 or higher)
- RStudio (recommended)

### Required R Packages
```r
# Install required packages
install.packages(c(
  "tidyverse",
  "flexdashboard",
  "gt",
  "htmltools",
  "viridisLite",
  "viridis",
  "dplyr",
  "plotly",
  "highcharter",
  "ggplot2",
  "scales",
  "RColorBrewer"
))
```

### Setup Instructions
1. Clone or download this repository
2. Open RStudio
3. Set the working directory to the project folder
4. Install required packages (if not already installed)
5. Open any `.Rmd` file and click "Knit" to generate HTML dashboards

## 🚀 Usage

### Running Individual Dashboards
1. **Comprehensive Suicide Analysis**: Open `Suicide_Data_Analysis.Rmd`
2. **Enhanced Laptop Analysis**: Open `Laptop_Story_Enhanced.Rmd`
3. **Combined Dataset Analysis**: Open `Combine_Two_DataSet.html` (pre-rendered)

### Generating HTML Output
```r
# In RStudio, click the "Knit" button
# Or use the command line:
rmarkdown::render("Suicide_Data_Analysis.Rmd")
rmarkdown::render("Laptop_Story_Enhanced.Rmd")
```

## 📈 Dashboard Features

### Suicide Data Analysis Dashboard (`Suicide_Data_Analysis.Rmd`)

![Suicide Data Analysis Dashboard](screenshots/Suicide%20Data.png)

*Comprehensive suicide data analysis dashboard featuring global overview, country-wise analysis, gender distribution, age group trends, and economic factors visualization*

- **Global Suicide Overview**: Key metrics and statistics
- **Top Countries by Total Suicides**: Interactive horizontal bar chart
- **Suicide Rate Trends Over Time**: Time series analysis with trend lines
- **Gender Analysis**: Donut chart showing suicide distribution by sex
- **Suicide by Age Group**: Bar chart of suicide rates across age groups
- **Economic Factors Analysis**: Scatter plot of GDP vs suicide rates
- **Decade Analysis**: Temporal trends across different decades
- **Geographic Heatmap**: Country-wise suicide rates by decade
- **Statistical Summary**: Comprehensive analysis by gender and age

### Enhanced Laptop Data Dashboard (`Laptop_Story_Enhanced.Rmd`)

![Laptop Data Analysis Dashboard](screenshots/Laptop%20Data.png)

*Enhanced laptop data analysis dashboard featuring 3D visualizations, interactive heatmaps, bubble charts, and advanced styling with modern gradients*

- **3D Scatter Plots**: Price vs Rating vs RAM relationships
- **Interactive Heatmaps**: Brand performance visualization
- **Bubble Charts**: Multi-dimensional data representation
- **Radar Charts**: Brand comparison across multiple metrics
- **Advanced Styling**: Modern gradients and animations

### Combined Dataset Dashboard
- **Top Selling Laptop Brands Rating**: Pie chart of brand ratings
- **Country-wise Suicide Data**: Interactive world map with suicide rates
- **Best Display Sizes**: Bar chart of popular laptop display sizes

## 🎨 Visualization Libraries Used

- **Plotly**: Interactive plots and charts with hover effects
- **Highcharter**: Interactive maps and advanced charts
- **ggplot2**: Static visualizations with enhanced themes
- **Viridis**: Color palettes for accessibility and aesthetics
- **Flexdashboard**: Dashboard layout and structure
- **Custom CSS**: Modern styling with gradients and animations

## 📝 Key Insights

### Suicide Data Analysis
- **Gender Disparity**: Males consistently show higher suicide rates than females across all age groups
- **Age Vulnerability**: Middle-aged adults (35-54 years) show the highest suicide rates
- **Geographic Patterns**: Significant variations in suicide rates across countries and regions
- **Economic Factors**: Complex relationship between GDP and suicide rates
- **Temporal Trends**: Changing patterns across decades indicating social and policy impacts

### Laptop Market Analysis
- **Brand Performance**: Clear differences in ratings and popularity across brands
- **Price-Performance**: Relationship between laptop specifications and pricing
- **Consumer Preferences**: Display size and storage preferences
- **Market Trends**: Evolution of laptop specifications over time

## 🎨 Design Features

### Enhanced Styling
- **Gradient Backgrounds**: Modern color schemes with smooth transitions
- **Hover Effects**: Interactive elements with smooth animations
- **Custom Animations**: Fade-in effects and pulse animations
- **Responsive Design**: Adapts to different screen sizes and devices
- **Professional Typography**: Clean, readable fonts with proper hierarchy

### Interactive Elements
- **Hover Information**: Detailed tooltips with additional data
- **Zoom and Pan**: Interactive chart controls
- **Color-coded Visualizations**: Consistent color schemes across charts
- **Dynamic Updates**: Real-time data processing and visualization

## 🤝 Contributing

Feel free to contribute to this project by:
- Adding new visualizations and chart types
- Improving data analysis and statistical insights
- Enhancing dashboard layouts and user experience
- Adding new datasets and analysis perspectives
- Improving CSS styling and animations

## 📄 License

This project is open source and available under the MIT License.

## 👨‍💻 Author

Created as a data visualization project demonstrating R's capabilities in creating interactive dashboards and data analysis.

---

**Note**: This project is for educational and demonstration purposes. The suicide data should be handled with sensitivity and used responsibly for research and awareness purposes. The visualizations are designed to provide insights while maintaining appropriate sensitivity to the subject matter.