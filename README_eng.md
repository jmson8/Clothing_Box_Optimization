# Optimal Location Selection for Clothing Boxes in Gwangjin District
## Analysis Overview

### Research Background
- Growing importance of systematic management of clothing boxes due to increasing textile waste (Fast Fashion).
- Lack of proper management of clothing boxes in Gwangjin District, leading to aesthetic issues.
- Need to improve accessibility to clothing boxes across different neighborhoods.

### Analysis Data
1. **Population Data**

    | Year | Data Name | Purpose | Source |    
    |------|-----------|---------|--------|  
    | 2024 | Seoul Population by Census Block (Korean Nationals) | Analyze regional population distribution | Seoul Open Data Plaza |
    | 2024 | Seoul Population by Administrative District (Korean Nationals) | Analyze regional population distribution | Seoul Open Data Plaza |
    | 2023 | Resident Population (by gender and age) | Identify age-specific population distribution | Seoul Metropolitan Basic Statistics |
    | 2022 | Gwangjin District Population by Grid | Analyze population distribution by grid unit | National Spatial Information Portal |

2. **Administrative Data**

    | Year | Data Name | Purpose | Source |    
    |------|-----------|---------|--------|  
    | 2024 | Administrative District Boundary | Verify regional boundary criteria | Seoul Open Data Plaza |
    | 2024 | Locations of Clothing Boxes in Gwangjin | Identify locations of clothing boxes | Public Data Portal |
    | 2022 | Administrative District Statistics (by neighborhood) | Analyze area distribution by neighborhood | Seoul Metropolitan Statistics |
    | 2021 | Building Classification by Use | Analyze building distribution by type | Building Lifecycle Management System |

3. **Consumption Data**

    | Year | Data Name | Purpose | Source |    
    |------|-----------|---------|--------|  
    | 2023 | Seoul Clothing Consumption Trends | Analyze clothing consumption patterns by gender/age | DATUS |

### Analysis Tools
- `Python`: Data preprocessing, visualization, and P-median analysis
- `QGIS`: Creation and visualization of spatial data
- `Tableau`: Exploratory data analysis and visualization

## Analysis Contents
### Algorithm
- P-median Algorithm: A location-allocation model minimizing distances between candidate sites and demand locations.

### Analysis Process
1. **Current Status of Clothing Boxes** 
   - Review population and building distribution in Gwangjin District.
   - Assess current installation status of clothing boxes in Gwangjin District.
   - Examine age-specific clothing consumption trends and notable patterns.

2. **Creating Derived Variables** 
   - Generate a Clothing Consumption Index: clothing purchase count by age group.
   - Create a Clothing Box Demand Index: considering population, area, and building count.

3. **Applying the P-median Model** 
   - Standardize derived variables to create a final index, considering both the Clothing Consumption Index and Clothing Box Demand Index.
   - Decide whether to add or remove clothing boxes based on the final index in relation to current box numbers.
   - Use the P-median model to generate node locations and identify nodes requiring addition/removal of boxes.

### Analysis Results
- Areas Requiring Additional Clothing Boxes: Jayang 3-dong, Gwangjang-dong, Jayang 4-dong, Hwayang-dong.
- Areas Requiring Removal of Clothing Boxes: Jayang 2-dong, Guui 2-dong, Neung-dong, Jayang 1-dong.

### Utilization and Expected Benefits
- Improved accessibility to clothing boxes, enhancing user convenience.
- Reduced socioeconomic costs through efficient operation of clothing boxes.
- Real-time information on clothing boxes accessible to the public.
