
# Global Energy Project
An interactive Tableau data visualization project exploring global energy consumption patterns, renewable energy growth, and the transition from fossil fuels to clean energy sources across continents and countries from 1970 to 2025.

## Dataset
https://lowcarbonpower.org/data-including-net-imports.csv

**Key Metrics**:
- Total Energy Consumption (TWh)
- Fossil Fuel Energy (TWh)
- Renewable Energy (TWh)
- Nuclear Energy (TWh)

**Geographic Coverage**: 
- 200+ countries
- 6 continents
- Regional and continental aggregations

**Temporal Coverage**: 1970-2025

### Energy Type Classification
The dataset contains various energy types organized in a hierarchical structure. Below is a comprehensive breakdown:

#### Top-Level Aggregations
| Energy Type | Description |
|-------------|-------------|
| `total` | All energy sources combined |
| `primary` | Primary energy from natural sources before conversion |
| `trade` | Energy imports and exports |

### Major Categories
| Energy Type | Description |
|-------------|-------------|
| `fossil` | All fossil fuels (coal + oil + gas) |
| `renewables-including-hydro` | All renewable energy sources |
| `nuclear` | Nuclear energy |

### Fossil Fuels
| Energy Type | Description |
|-------------|-------------|
| `coal` | Coal energy |
| `oil` | Petroleum and crude oil |
| `gas` | Natural gas |
| `unspecified-fossil-fuels` | Fossil fuels not otherwise categorized |

### Renewable Energy Sources
| Energy Type | Description |
|-------------|-------------|
| `hydro` | Hydroelectric power |
| `wind` | Wind power |
| `solar` | Total solar energy |
| `solar-utility` | Utility-scale solar farms |
| `solar-btm` | Behind-the-meter solar (rooftop/distributed) |
| `wind-and-solar` | Wind and solar combined |
| `geothermal` | Geothermal energy |
| `biofuels` | Biomass and biofuel energy |
| `geothermal-and-biofuels` | Geothermal and biofuels combined |
| `unspecified-renewables` | Renewable sources not otherwise categorized |

### Lowcarbon
| Energy Type | Description |
|-------------|-------------|
| `lowcarbon` | Low-carbon sources (nuclear + renewables) |

### Primary Energy by End Use
Primary energy sources are further categorized by their end use:

**Electricity Generation (suffix: `-e`)**
- `primary-coal-e` - Coal used for electricity generation
- `primary-oil-e` - Oil used for electricity generation
- `primary-gas-e` - Natural gas used for electricity generation
- `primary-renewables-e` - Renewables used for electricity generation
- `primary-biofuels` - Biofuels for electricity

**Non-Electricity Use (suffix: `-ne`)**
- `primary-coal-ne` - Coal for non-electric purposes (heating, industrial processes)
- `primary-oil-ne` - Oil for non-electric purposes (transportation, heating, petrochemicals)
- `primary-gas-ne` - Natural gas for non-electric purposes (heating, industrial)
- `primary-renewables-ne` - Renewables for non-electric use (biofuels for transport)

### Other
| Energy Type | Description |
|-------------|-------------|
| `other` | Miscellaneous energy sources not fitting other categories |

### Column Definitions
| Column | Description |
|--------|-------------|
| ISO | ISO 3166-1 alpha-2 country code |
| Country | Country name |
| Energy Category | Type/category of energy (see Energy Type Classification) |
| Year | Year of measurement (1971-2025) |
| Energy (TWh) | Energy production/consumption in Terawatt-hours |

## Notebooks
1. **`01_data_preprocessing.ipynb`** – Data cleaning and preprocessing: handling missing values, type conversions, monthly aggregation, and dataset validation.

2. **`02_african_regions.ipynb`** – Crreating CSV containing African countries classified by ISO-codes and region.

3. **`03_continents.ipynb`** – Creating CSV containing countries classified by ISO-codes and continents.
   
## Visualizations

| Sheet Name | Visualization Type | Purpose |
|------------|-------------------|---------|
| Complete Picture| Bubble Chart | Overview of the global energy landscape|
| Energy Gap | Stacked Area Chart | The gap between fossil fuels and renewable energy across thre time periods |
| Energy Giants | Bar Chart | Top energy-consuming countries |
| Energy Mix | Stacked Bar Chart | Breakdown of energy sources by continent |
| Energy Source | Pie chart | Distribution of various sources of energy; coal, oil, hydro, biofuels etc |
| Energy Type | Stacked Area Chart | Comparison between fossil, renewable and nuclear energy overtime |
| Fossil Reality | Bar Chart |Current state of fossil dependent vs renewable transition and role of nuclear energy |
| Fossil Dependence | Horizontal Bar Chart | Continents dependency on fossil fuels and distance to renewable transition goal |
| Global Energy Consumption | Grouped Bar Chart | Total energy consumption trends worldwide over three periods |
| Global Energy Transition | Dashboard | Interactive Dashboard showing key energy metrics |
| Renewable Energy Share | Map | Geographic map showing renewable energy adoption by country |
| Renewable Revolution | Line Chart | Growth of renewable energy across three time periods |

##  Key Insights

- **Energy consumption has more than doubled** since 1995
- **USA and China** dominate global energy use
- **Renewable energy** has grown exponentially since 2010
- **Significant regional variation** in renewable adoption

## Visualizations Included

| Sheet Name | Visualization Type | Purpose |
|------------|-------------------|---------|
| Energy Growth | Grouped Bar Chart | Show energy consumption evolution across three periods |
| Top Energy | Horizontal Bar Chart | Rank countries by total energy consumption |
| Top Renewable | Horizontal Bar Chart | Identify renewable energy leaders |
| Top Fossil | Horizontal Bar Chart | Show fossil fuel dependency patterns |
| Top Nuclear | Horizontal Bar Chart | Display nuclear energy capacity leaders |
| Solar Energy Growth Rates | Heat Map | Visualize solar growth acceleration over time |
| Wind Energy Growth Rates | Heat Map | Track wind energy expansion patterns |
| Solar vs Wind Timeline | Dual-Axis Line Chart | Compare growth trajectories of both technologies |
| Energy Mix by Continent | Stacked Bar Chart | Show renewable vs. fossil composition by region |
| Growth Rate Comparison | Scatter Plot | Analyze solar vs. wind growth dynamics by country |

## Future Enhancements

### Planned Features

- [ ] Add per-capita energy consumption metrics
- [ ] Include energy intensity (energy per GDP) analysis
- [ ] Integrate carbon emissions data
- [ ] Add cost analysis (LCOE - Levelized Cost of Energy)
- [ ] Create mobile-optimized dashboard layouts
- [ ] Add predictive models for future energy mix
- [ ] Include hydroelectric and geothermal energy sources
- [ ] Add policy timeline overlays (Paris Agreement, etc.)

### Data Updates

- [ ] Automate data refresh from public sources
- [ ] Add real-time or quarterly data updates
- [ ] Include more granular geographic data (states/provinces)

## Tools
Python, Pandas, Tableau Public

## License

[ MIT]

## Author

[Kadi Sadaraka]

## Acknowledgments

- Dataset: Low Carbon Power yearly data

