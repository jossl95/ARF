# Artificial Reputation Formation

This depository contains all code that I used to analyse the [DNM archives](https://www.gwern.net/DNM-archives#download). In my analyses I will asses the effect of Artificial Reputation Formation on the market succes of cryptosellers. For this purpose I parsed the data on listing at 'SilkRoad2' market.  

## Getting Started
### Retrieving data
Download or clone this repository on your local machine to unpack, parse and mutate the data. The scripts in this repository have the following purpose
1. `Unpacker.ipynb` unpacks an decompresses all the data from the [tarball](https://archive.org/download/dnmarchives/dnmarchives_archive.torrent)
2. `Parser.ipynb` reads the folder structure as an dictionary and stores the data in a `.json` file. Then it parses: feedbacks, items and vendor information into designated data tables. These data tables are stored as `.pickle`, because this yields the shortest read and write speeds.

### Cleaning and preparing the data
3. `Cleaner.ipynb` cleans the data tables created in the parsing process. This cleaner aims to reduce memory usages and exclude duplicate cases and optimize data times.
4. `Operationalizer.ipynb` prepares and aggregates the data to a person-period file to facilitate statistical analyses
5. `Codebook.ipynb` describes the variables that are contained within the person-period file. 

### Analyses
6. `Analyzer.ipynb` transforms variables for analyses with a yeo-johnson transformation. The analyses are performed in `R` using `lme4`'s `glmer` function to estimate random-slope models. 
7. `Robustness.ipynb` additional analyses are performed to test the robustness of ARM operationalization. 

## License

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
