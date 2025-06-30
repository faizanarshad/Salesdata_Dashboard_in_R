# Sales Data Dashboard in R

A comprehensive data visualization project that combines multiple datasets to create interactive dashboards using R Markdown and Flexdashboard. This project analyzes both suicide data and laptop sales data, providing insights through various interactive visualizations.

## 📊 Project Overview

This project demonstrates advanced data visualization techniques in R, combining two distinct datasets:
- **Suicide Data**: Global suicide statistics from 1985-2015
- **Laptop Sales Data**: Laptop specifications and ratings from various brands

## 🎯 Features

### Interactive Visualizations
- **Pie Charts**: Brand ratings and suicide distribution by sex
- **Scatter Plots**: Suicide trends by age groups
- **Bar Charts**: Population vs suicide rates and display size distributions
- **World Maps**: Country-wise suicide data visualization
- **Interactive Plots**: Using Plotly and Highcharter libraries

### Dashboard Components
- **Flexdashboard**: Responsive layout with multiple columns
- **Real-time Data Processing**: Dynamic data manipulation and visualization
- **Color-coded Visualizations**: Using Viridis color palettes
- **Responsive Design**: Adapts to different screen sizes

## 📁 Project Structure

```
Salesdata_Dashboard_in_R/
├── README.md                           # This file
├── SucideData.csv                      # Global suicide statistics dataset
├── laptops.csv                         # Laptop specifications and ratings dataset
├── Project_Two.Rmd                     # Suicide data analysis dashboard
├── Project_Two.html                    # Compiled HTML version
├── Combine_Two_DataSet.Rmd             # Combined dataset dashboard
├── Combine_Two_Dataset.html            # Compiled HTML version
├── Worlds Population and Sucide Data_2.Rmd  # Laptop data analysis dashboard
├── Worlds Population and Sucide Data_2.html # Compiled HTML version
├── Worlds Population and Sucide Data.Rmd    # Additional suicide analysis
└── Worlds Population and Sucide Data.html   # Compiled HTML version
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
- `suicides/100k pop`: Suicide rate per 100,000 population
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
  "ggplot2"
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
1. **Suicide Data Analysis**: Open `Project_Two.Rmd`
2. **Combined Dataset Analysis**: Open `Combine_Two_DataSet.Rmd`
3. **Laptop Data Analysis**: Open `Worlds Population and Sucide Data_2.Rmd`

### Generating HTML Output
```r
# In RStudio, click the "Knit" button
# Or use the command line:
rmarkdown::render("Project_Two.Rmd")
rmarkdown::render("Combine_Two_DataSet.Rmd")
rmarkdown::render("Worlds Population and Sucide Data_2.Rmd")
```

## 📈 Dashboard Features

### Project Two Dashboard
- **Total Suicides Trend by Sex**: Interactive pie chart showing suicide distribution
- **Suicide Trends by Age**: Scatter plot of suicide rates vs age groups
- **Suicides by Country**: Bar chart of population vs suicide numbers

### Combined Dataset Dashboard
- **Top Selling Laptop Brands Rating**: Pie chart of brand ratings
- **Country-wise Suicide Data**: Interactive world map with suicide rates
- **Best Display Sizes**: Bar chart of popular laptop display sizes

### Laptop Data Dashboard
- **Laptop Sale (Brand Rating)**: Pie chart of brand ratings
- **Top Selling Brands**: Interactive scatter plot of top brands
- **Best Laptop Display**: Bar chart of display size distribution

## 🎨 Visualization Libraries Used

- **Plotly**: Interactive plots and charts
- **Highcharter**: Interactive maps and advanced charts
- **ggplot2**: Static visualizations
- **Viridis**: Color palettes for accessibility
- **Flexdashboard**: Dashboard layout and structure

## 📝 Key Insights

### Suicide Data Analysis
- Gender-based suicide patterns
- Age group vulnerability analysis
- Geographic distribution of suicide rates
- Temporal trends over 30 years

### Laptop Market Analysis
- Brand popularity and ratings
- Price-performance relationships
- Display size preferences
- Market trends and consumer behavior

## 🤝 Contributing

Feel free to contribute to this project by:
- Adding new visualizations
- Improving data analysis
- Enhancing dashboard layouts
- Adding new datasets

## 📄 License

This project is open source and available under the MIT License.

## 👨‍💻 Author

Created as a data visualization project demonstrating R's capabilities in creating interactive dashboards and data analysis.

---

**Note**: This project is for educational and demonstration purposes. The suicide data should be handled with sensitivity and used responsibly for research and awareness purposes.