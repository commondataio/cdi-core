# cdi-core

Common Data Index is a registry and search index of all public data catalogs, catalogs metadata, search index and data storage/backup.

This repository holds roadmap, architecture and high-level tasks

Please take a look at [project mindmap](/assets/commondataindex.png) to see it's goals and structure.


## Quick links

* [Data catalogs registry dataset](https://github.com/commondataio/dataportals-registry/blob/main/data/datasets/catalogs.jsonl)


### Q&A


## What for is this project?

This project started as open source foundation of open source, open data alternative to [Google Dataset search](https://datasetsearch.research.google.com/). 

Alternatively to Google Dataset search it provides API access to whole search index and allows to use more complex search queries using combination of data source metadata, datasets metadata and metadata extracted from data itself.

## What makes it different?

Google Dataset search is built around Schema.org [Dataset](https://schema.org/Dataset) schema of structured data. It's easier to implement for classic search engines like Google, since it's already crawl whole Internet, but it's much less usable for any other data aggregation project.

At the same time most data portals in the world support one or more ways (APIs) to work with metadata or data. For example, it's CKAN API, Dataverse API, [DCAT](https://www.w3.org/TR/vocab-dcat-3/#Class:Distribution), OpenDataSoft and API/data export by many other vendors and open source products. 

A lot of data portals, especially open geodata catalogs do not support Schema.org and do not support web crawlers since they are use API-based page rendering. For example GeoNode and Geonetwork instances couldn't be crawled by common web crawlers and do not support Schema.org. 

Instead of using Schema.org markup Common Data Index harvests metadata from data catalogs and converts collected metadata to the unified search index.

## Project outputs

Following products are results of this porject:
1. Registry of data portals as dataset, API and web UI.
2. Knowledge base about how data published, data and metadata standards, data portals types and so on.
3. Database of raw indexes available as bulk data and via API
4. Search index database available via API.
5. Search engine UI.

Additional possible output is an open source harvester to collect metadata and files from data catalogs.

## What kind of data catalogs collected?

Following data portals type:
* **Open data portals** - most of them about open data published by government and based on CKAN, DKAN, uData, JKAN software
* **Geoportals** - public geodata catalogs like Geonetwork, GeoNode, ArcGIS Hub and ArcGIS Server
* **Scientific data repositories** - repositories used to publish open research data, common software is Dataverse, InvenioRDM and many types of institutional research output repostitories like DSpace, EPronts and e.t.c.
* **Indicators catalogs** - data catalogs or databases that provide access to statistical data by indicator. Most often they are PxWeb or .Stat based.
* **Microdata catalogs** - data catalogs with statistical survey's microdata. Most of them based on NADA open source data catalog, not always open data, sometimes only metadata available
* **Machine learning catalogs** - data catalogs for machine learning purposes, no common software, mostly online projects like Hugging Face and Kaggle 
* **Data search engines** - search engines to search data
* **API Catalogs** - catalogs of API, with data-related API in focus
* **Data marketplaces** - commercial data catalogs, only metadata and sometimes data samples available
* **Other** - any other data catalog


