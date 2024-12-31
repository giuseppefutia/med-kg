# med-kg
Building Your Medical Knowledge Graph (med-kg), One Dataset at a Time. 

## Project Details
The goal of this repository is to provide a comprehensive guide for constructing a biomedical knowledge graph by integrating multiple datasets into a unified graph representation using Neo4j.

## Neo4j Plugins
To build your med-kg in Neo4j, you have to install the following plugins:
* Graph Data Science (GDS)
* Neosemantics

## Python Requirements
`Makefile` assumes you have a virtual environment folder called `venv` 
at the repository root folder. 

You can create and activate your virtual environment with the following code:

```shell
virtualenv -p python3 venv
source venv/bin/activate
```

You can edit the`Makefile` and redefine the `PIP` variable at the first line to match your configuration. Then, you can run the following command to install all the required Python libraries.
```shell
cd importer
make init
```

## Dataset Exploration
In the `explorer` folder, you will find notebooks to run explorative analysis of the source data.

## Dataset Importing
Run this commands to execute the importer code for each dataset.
```shell
cd importer
make import
```

## Graph-based Analysis
In the `analyzer` folder, you will find notebooks to run graph-based analysis on the resulting biomedical knowledge graph.