# Daily R<sub>e</sub> for select countries

See https://ibz-shiny.ethz.ch/covid-19-re/ for an interactive visualisation of the data.

See https://ibz-shiny.ethz.ch/covid-19-re/methods.pdf for an explanation of the method used.

## Data Format

Data is provided as a csv per country named with the countries [alpha-3 code](https://www.iso.org/obp/ui/#search) + `-estimates.csv``

The data contains the following columns:

| column name      | value              | description                                    |
|------------------|--------------------|------------------------------------------------|
| country          | string             | country name                                   |
| region           | string             | region (e.g. Province, Canton etc.)            |
| source           | string             | data source abbreviation (see dataSources.csv) |
| data_type        | string             | Data type on which the estimation is based on  |
| estimate_type    | string             | Estimation type (sliding window or step-wise)  |
| date             | string, YYYY-MM-DD | Date                                           |
| median_R_mean    | float              | mean estimated median R<sub>e</sub>            |
| median_R_highHPD | float              | upper bound of the 95% confidence interval     |
| median_R_lowHPD  | float              | lower bound of the 95% confidence interval     |
| countryIso3      | string             | alpha-3 country code                           |
