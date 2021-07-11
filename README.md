# GeneSearchService

This is a simple RESTful service with a single endpoint "gene_suggest", used for querying genes by prefix and species.

## Usage

After cloning this repo, sync your Python virtual environment with the ```requirements.txt``` file.

Then run ```python main.py``` on a windows machine or ```./main.py``` on Unix.  This should start the
service on localhost on port 5000.  Here is an example query to run against the gene_suggest endpoint:

```
http://localhost:5000/gene_suggest?query=BRC&species=homo_sapiens&limit=10
```

This should return a list:

```["BRCA1", "BRCA2", "BRCC3", "BRCC3P1"]```

## Testing

```pytest test.py```