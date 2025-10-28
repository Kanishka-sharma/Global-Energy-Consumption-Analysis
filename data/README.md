# Project Data

The `energy.csv` dataset used for this project is from a private source and cannot be shared publicly.

## Data Schema

The analysis code in this repository requires a file named `energy.csv` in this directory. The file must have the following structure:

* **`country`**: (character) The name of the country.
* **`year`**: (integer) The year of the observation (1996-2023).
* **`iso_code`**: (character) The 3-letter country code.
* **`population`**: (numeric) The total population.
* **`gdp`**: (numeric) The Gross Domestic Product.
* **`fossil_fuel`**: (numeric) Energy from fossil fuels (TWh).
* **`nuclear`**: (numeric) Energy from nuclear (TWh).
* **`primary_energy`**: (numeric) Total primary energy (TWh).
* **`renewables`**: (numeric) Energy from renewables (TWh).

While the analysis cannot be run without this private file, the code is provided to demonstrate the methodology and analytical process.