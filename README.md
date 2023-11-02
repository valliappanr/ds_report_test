# This project is to generate a report of processing two datasets and aggregate the data of the two datasets

## Below are the requirements for the report,

```Please do same exercise using two different framework.

Framework 1. pandas
framework 2. apache beam python https://beam.apache.org/documentation/sdks/python/


using two input files dataset1 and dataset2 

join dataset1 with dataset2 and get tier

generate below output file

legal_entity, counterparty, tier, max(rating by counterparty), sum(value where status=ARAP), sum(value where status=ACCR)

Also create new record to add total for each of legal entity, counterparty & tier.

Sample data:
legal_entity, counterparty, tier, max(rating by counterparty), sum(value where status=ARAP), sum(value where status=ACCR)
L1,Total, Total, calculated_value, calculated_value,calculated_value
L1, C1, Total,calculated_value, calculated_value,calculated_value
Total,C1,Total,calculated_value, calculated_value,calculated_value
Total,Total,1,calculated_value, calculated_value,calculated_value
L2,Total,Total,calculated_value, calculated_value,calculated_value

like all other values.

where caluclated_value in sample data needs to be calculated using above method.```


## Assumptions

* All the aggregations are carried out based on the unique values for legal_entity, counter_party, tier
* Again the total elements were calculated based on unique values for legal_entity, counter_party, tier

## Two Notebooks created

1. gen_report_pandas.ipynb - for pandas implementation
2. gen_report_beam.ipynb - for Apache Beam implementation


