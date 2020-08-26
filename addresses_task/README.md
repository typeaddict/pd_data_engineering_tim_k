# Data Engineering hiring

This is an intro data engineering task for candidates

## Instructions

### Task

Your task is to identify duplicates between addresses (as much as possible), extract country and city for each address

We expect from you `addresses.csv` file with columns [`address`, `city`, `country`] without duplicates (you might need additional columns that you will use for deduplication, if so please include them in the final file) and jupyter notebook with code

### Data

You have `addresses.csv` with raw addresses inside

Files:
* `data/addresses.csv` contains next columns: `addresses`

### Tips

* once you identify the country please use its alpha-2 code instead, for example: 'Switzerland' -> 'CH'
* sometimes several addresses have different department name inside but the same root e.g.

| address | root |
| ------ | ------ |
| `Department of Pharmaceutical Sciences, University Basel, 4056 Basel, Switzerland` | `University Basel, Basel, Switzerland` |
| `Department Biomedicine, University Basel, 4056 Basel, Switzerland` | `University Basel, Basel, Switzerland` |

in this case, we can assume that these 2 addresses are the same, because they have identical roots


# Submission 

Write your code in the develop branch and submit a MergeRequest to @igor7pro to us once you're done.