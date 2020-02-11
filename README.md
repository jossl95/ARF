# Thesis

This depository contains all code that I used to analyse the [DNM archives](https://www.gwern.net/DNM-archives#download) for my thesis. In my analyses I will asses the effect of Artificial Reputation Formation on the market succes of cryptosellers. For this purpose I scraped the data on listing at 'SilkRoad2' market.  

## Getting Started

Download or clone this repository on your local machine to unpack, parse and mutate the data. The scripts in this repository have the following purpose
1. `Unpacker.ipynb` unpacks an decompresses all the data from the [tarball](https://archive.org/download/dnmarchives/dnmarchives_archive.torrent)
2. `Parser.ipynb` reads the folder structure as an dictionary and stores the data in a `.json` file. Then it parses: feedbacks, items and vendor information into designated data tables. These data tables are stored as `.pickle`, because this yields the shortest read and write speeds. 
3. `Cleaner.ipynb` cleans the data tables created in the parsing process. This cleaner aims to reduce memory usages and exclude duplicate cases.
