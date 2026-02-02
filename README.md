# Global Energy Transition Dashboard
Interactive Tableau dashboard analyzing global energy transition trends.

## Data
Multi-country, multi-year energy data by source.

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
| `lowcarbon` | Low-carbon sources (nuclear + renewables) |
| `renewables-including-hydro` | All renewable energy sources |
| `renewables-except-hydro` | Renewable sources excluding hydroelectric |

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

### Nuclear
| Energy Type | Description |
|-------------|-------------|
| `nuclear` | Nuclear energy |

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
| Energy Type | Type/category of energy (see Energy Type Classification) |
| Year | Year of measurement (1971-2025) |
| Energy (TWh) | Energy production/consumption in Terawatt-hours |

### Data Scale
- **Unit**: Terawatt-hours (TWh)
- **1 TWh** = 1,000,000,000 kWh (1 billion kilowatt-hours)

## Methods
- Data cleaning & feature engineering in Python
- Energy dependency and transition metrics
- Interactive dashboards in Tableau Public

## Key Insights
- Renewable growth is uneven across regions
- Some oil-dependent countries show rapid transition
- Trade dependency correlates with energy vulnerability

## Tools
Python, Pandas, Tableau Public
