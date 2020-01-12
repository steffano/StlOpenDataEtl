# StlOpenDataEtl

_Author_: @nicseltzer

_Status_: Planning

## Description

This project aims to be the jumping off point for the OpenSTL Extract, Transform, and Load (ETL) pipeline.

##  Developing

The below notes assume that you've forked the repo to your account and have pulled down a clone of that fork.

Note: This project has only been built on MacOS and Linux so far. Submit PRs with instructions on building / running in Windows (or whatever you use).

### Get Python3

If you don't have Python3 installed, you'll need to download it from the [Python website](https://www.python.org/downloads/) for your particular operating system.

### Setup your Virtual Environment (venv)

There are a lot of resources for doing this online, but I recommend the following (espeically if you're using VSCode):

#### Virtual Environment

1. From your locally cloned repo, run `python3 -m venv .venv`. This will create a .venv directory which contains all of the pieces for your local Python project.
1. That's it. You've created a venv.


#### Activating Virtual Environment

1. Using the your favorite terminal or the terminal built-in to VSCode (which should pick up `.venv` automatically), run `source ./.venv/bin/activate`. This will do the magic of setting up your project in isolation from your global package manifest.
1. Next, we need to get the dependencies for the project. You can do this by running `./make.py`. If you need to add dependencies, you can add them with `pip` as you normally would. Just make sure to run `./package.py` before committing back to the repo.

#### Running The Application

1. Run `python3 ./app.py`.


#### Deactivating Virtual Environment

1. Run `deactivate`.


## Components

### Fetcher

_Author_: @nicseltzer

_Status_: Under Development

This script is run at a configurable interval and is responsible for fetching data from configured remote sources.

### Extractor

_Author_: Looking for owner

_Status_: Unstarted

### Transformer

_Author_: Looking for owner

_Status_: Unstarted

### Loader

_Author_: Looking for owner

_Status_: Unstarted

## Remote Data Sources

### Parcels (Shape, used for Key: HANDLE)

https://www.stlouis-mo.gov/data/upload/data-files/prcl_shape.zip

### Parcels (Information)

### Includes Tax Billing Information

https://www.stlouis-mo.gov/data/upload/data-files/prcl.zip
https://www.stlouis-mo.gov/data/upload/data-files/par.zip

### LRA Inventory

https://www.stlouis-mo.gov/data/upload/data-files/lra_public.zip

### Building Inspections

### Includes Condemnations and Vacant buildings

https://www.stlouis-mo.gov/data/upload/data-files/bldginsp.zip

### Building Permits

### Includes Occupancy and Demolition

https://www.stlouis-mo.gov/data/upload/data-files/prmbdo.zip

### Property Maintenance Billing (Using Forestry Property Maintenance)

https://www.stlouis-mo.gov/data/upload/data-files/forestry-maintenance-properties.csv
