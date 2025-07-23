# AWS Community Data Analytics Project

This project provides tools for analyzing and visualizing data about AWS Heroes and Community Builders, offering insights into the global AWS community ecosystem.

## Overview

The AWS Community Data Analytics project collects, cleans, and analyzes data about AWS Heroes and Community Builders worldwide. It provides insights into their geographical distribution, specializations, and community contributions.

To interact with the visualization follow these links:

- **AWS Community Builders:** [Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMTc4Mzk2NGUtZDdhYS00NWNiLWI5MTAtYTE1MmM3YjFjZGUzIiwidCI6Ijc0NDczNDI5LTA5ODMtNDg1OS04ZDU5LWJlODRhNzRjZmFkOCJ9)

<img width="1087" height="592" alt="Screenshot from 2025-07-24 02-11-03" src="https://github.com/user-attachments/assets/d6ae7bbd-fa80-4315-bc7d-08c63141432e" />

- **AWS Heroes:** [Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNDM5YTA2ZTYtMWVhYS00NWEyLWFiNmEtNjQwNGI1OTgzMGU1IiwidCI6Ijc0NDczNDI5LTA5ODMtNDg1OS04ZDU5LWJlODRhNzRjZmFkOCJ9)

<img width="1042" height="601" alt="Screenshot from 2025-07-24 02-11-39" src="https://github.com/user-attachments/assets/637a35c7-ba4d-4de1-880c-7ce349fcf916" />

- **AWS User Groups:** Coming Soon...

## Project Structure

```txt
aws_cleaned_data/
├── data/                      # Data files
│   ├── aws_heroes_cleaned.csv # Cleaned AWS Heroes data
│   ├── community_builders.csv # Cleaned Community Builders data
│   └── country_regions.json   # Country to region mapping
├── notebooks/                 # Jupyter notebooks
│   ├── clean_cb_data.ipynb    # Community Builders data cleaning
│   └── clean_heroes_data.ipynb # AWS Heroes data cleaning
├── scripts/                   # Python scripts
│   └── main.py                # Main script
├── pyproject.toml            # Project dependencies and metadata
└── .env                       # Environment variables
```

## Data Description

### AWS Heroes

The AWS Heroes program recognizes individuals who make significant contributions to the AWS community. The dataset includes:

- Hero profiles with names, locations, and categories
- Hero specializations (DevTools, Serverless, Container, etc.)
- Geographical information (country and region)
- Community contributions (Conference Speaker, Blogger, etc.)
- Active status (Current or Former Heroes)

### Community Builders

The AWS Community Builders program supports individuals who are actively sharing AWS knowledge. The dataset includes:

- Builder profiles with anonymized IDs
- Builder specializations (Serverless, Machine Learning, etc.)
- Geographical information (country and region)
- Year of joining the program

## Getting Started

### Prerequisites

- Python 3.11 or higher
- Required Python packages (see below)

### Installation

1. Clone the repository
2. Install dependencies using `uv` (recommended):

```bash
uv pip install -e .
```

If you don't have `uv` installed, you can install it following the instructions at [https://github.com/astral-sh/uv](https://github.com/astral-sh/uv).

Alternatively, you can use pip:

```bash
pip install -e .
```

### Dependencies

All dependencies are specified in the `pyproject.toml` file and include:

- ipykernel>=6.29.5
- pandas>=2.3.0
- pycountry>=24.6.1
- python-dotenv>=1.1.1
- requests>=2.32.4

## Data Analysis

The project includes Jupyter notebooks for data cleaning and analysis:

- `notebooks/clean_heroes_data.ipynb`: Cleans and transforms AWS Heroes data
- `notebooks/clean_cb_data.ipynb`: Cleans and transforms Community Builders data

## Data Insights

The cleaned datasets allow for various analyses:

- Geographic distribution of AWS Heroes and Community Builders
- Trends in community growth over time
- Popular specializations and expertise areas
- Community contribution patterns

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- AWS for providing the Heroes and Community Builders programs
- Contributors to the open-source libraries used in this project

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Contact

If you have any questions or feedback about this project, please open an issue in the repository.

## Future Work

- Implement time-series analysis to track community growth
- Develop predictive models for community trends
- Add API integration for real-time data updates
