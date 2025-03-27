# challenge-ai
# Account Hierarchy Validator Challenge


## Overview
This challenge involves creating a system to validate hierarchical account relationships in financial statements. The system processes financial data where accounts have hierarchical relationships (parent-child) and validates that the sum of child account values equals their parent account value.

## Problem Description
Based on the file **itr_cia_aberta_DRE_con_2023.csv** in this repository, explore the given financial statement data and follow the instructions:
1. Process entries where `ORDEM_EXERC` is "ÚLTIMO"
2. Filter for specific `CNPJ_CIA`
3. Validate that parent account values equal the sum of their child accounts

### Example
For the following data:
```
CNPJ_CIA 00.000.000/0001-91
Account 3.11 = 7,290,982
Account 3.11.01 = 6,691,197
Account 3.11.02 = 599,785
```

The validation should confirm that:
```
3.11 = 3.11.01 + 3.11.02
7,290,982 = 6,691,197 + 599,785
```

