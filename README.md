# Thesis

This depository contains all code that I used to analyse the [DNM archives](https://www.gwern.net/DNM-archives#download) for my thesis. In my analyses I will asses the effect of Artificial Reputation Formation on the market succes of cryptosellers. For this purpose I scraped the data on listing at 'SilkRoad2' market.  

## Getting Started

Download or clone this repository on your local machine to unpack, parse and mutate the data. The scripts in this repository have the following purpose
1. `Unpacker.ipynb` unpacks an decompresses all the data from the [tarball](https://archive.org/download/dnmarchives/dnmarchives_archive.torrent)
2. `Parser.ipynb` reads the folder structure as an dictionary and stores the data in a `.json` file. Then it parses: feedbacks, items and vendor information into designated data tables. These data tables are stored as `.pickle`, because this yields the shortest read and write speeds.
3. `Cleaner.ipynb` cleans the data tables created in the parsing process. This cleaner aims to reduce memory usages and exclude duplicate cases.

## license

Copyright 2020 Jos Slabbekoorn

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
