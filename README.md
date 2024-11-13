# med-kg
Building Your Medical Knowledge Graph (med-kg), One Dataset at a Time.

## Required Neo4j Plugins
To build your med-kg in Neo4j, you have to install the following plugins:
* Graph Data Science (GDS)
* Neosemantics

## Install Python Requirements
`Makefile` assumes you have a virtual environment folder called `venv` 
at the repository root folder. 

You can create and activate your virtual environment with the following code:

```shell
virtualenv -p python3 venv
source venv/bin/activate
```

You can edit the`Makefile` and redefine the `PIP` variable at the first line to match your configuration. Then, you can run the following command to install all the required Python libraries.
```shell
make init
```

## Import Datasets
Run this commands to execute the importer code for each dataset.
```shell
cd importer
make import
```
