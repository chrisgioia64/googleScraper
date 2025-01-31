## Overview

The goal is to find the appropriate website for each government entity in the United States by using a Google search.
Currently, it is limited to Texas government entities. The main script is located at `search.py`.

### Program Flow

We read the Texas government entities from the first tab of `data/Texas Local Governments.xlsx`, perform a Google search query using the entity name, and use some domain-specific logic to either return a suitable url or no url. The results are written to a `data/texas_websites_...xlsx` file (the most recent is `texas_websites_01_10_22.xlsx`).

### Manual Overrides

If there is a government entity that returns an incorrect url under the current algorithm, you can override the url returned by adding an entry to the csv file `overrides/overriden_entities.csv`. Provide the entity name _exactly_ as it appears in column A of the resultant `data/texas_websites_...xlsx` file.

### Set Up

To install the necessary dependencies, run:

```
pip install -r requirements.txt
```
