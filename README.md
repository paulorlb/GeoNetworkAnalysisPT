
# Geo Network Preprocessing

This project is concerned with use cases of geo network preprocessing using Open Street Maps data and a Pythonic framework. The project is mainly focused on Portugal, despite it can be easilly adapted to the another places.
The work is inspired in different projects around the web related to the same topic looking to compile a set of different approaches in a single place, in order to answer the challenges of different use cases.
Most of this work is used by the author in its daily work at [Universidade de Aveiro](www.ua.pt) and [INEGI](http://www.inegi.pt/en/), and it is shared here in order to help others in the same situation.

-- State of the project: [UNDER DEVELOPMENT]

## Objectives

The content developed here is developed through the following objectives:

- Retrieve network ("roads") data from Open Street Maps in different ways, namely:
  - Using bounding boxes (e.g.: spatial geometric polygons, for example for defined administrative boundaries);
  - Processing data dumps from Open Street Maps database (e.g. [pbf](https://wiki.openstreetmap.org/wiki/PBF_Format) files);
- Pre-processing data to ensure routing calculations
  - Using offline tools
    - Based [OSMNx](https://osmnx.readthedocs.io/en/stable/) library;
    - Based on alternatives (e.g. [Pandana](https://udst.github.io/pandana/) );
    - Based on Open Source Routing Machine [OSRM](http://project-osrm.org/) and its python interface [pyosrm](https://pypi.org/project/pyosrm/) - under development - see this [tutorial](https://afi.io/blog/introduction-to-osrm-setting-up-osrm-backend-using-docker/) for an example which will be reproduced here later for the portuguese case;
  - Using online tools
    - Based on paid APIs (such as Google Maps, Bing Maps, etc.), using the [routingpy](https://routingpy.readthedocs.io/en/latest/) api as a wrapper for different API providers.


### Technology Stack

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)

## Requirements

- The author adopted [Mamba](https://mamba.readthedocs.io/en/latest/index.html) to manage the project libraries environment. To better reproduce that environment, the user can replicate it using the provided `GeoNetworkAnalysisPT.yml` file at the environment folder of the project. 
- To create the environment, run the following command on the terminal, inside the project folder (note that to this command to work, the user must have the mamba PATH added in its OS system environment variables; however, when install mamba through the miniforge distribution, it is provided a miniforge terminal, which can be used instead) 

```bash
mamba env create -f ./environment/GeoNetworkAnalysis.yaml
```

### Author

- [Paulo Batista](https://github.com/paulorlb]) 
  
Scientific CV at:  [CIÊNCIAVITAE](https://www.cienciavitae.pt//en/021C-1C53-E0DA)
