# Data Pipeline Research: ETL vs ELT vs EtLT
## ETL (Extract, Transform, Load)
ETL is a traditional data integration process where data is:
1. Extracted from source systems
2. Transformed into a structured format
3. Loaded into a data warehouse

### Process Flow
Source → Extract → Transform → Load → Data Warehouse

### Compliance Benefits
ETL supports compliance because:
- Data is cleaned before storage
- Sensitive data can be masked
- Data validation occurs early
- Reduced risk of storing non-compliant data

### Industry Example
Healthcare industry:
Patient data is extracted, anonymized, and then loaded into the data warehouse to comply with privacy laws.

### Advantages
- Strong compliance control
- High data quality
- Secure data handling

### Disadvantages
- Slower processing
- Less scalable


## ELT (Extract, Load, Transform)
ELT is a modern approach where data is:
1. Extracted
2. Loaded into storage
3. Transformed later

### Process Flow
Source → Extract → Load → Transform → Data Warehouse

### Compliance Considerations
ELT introduces compliance risks because:

- Raw data is stored first
- Sensitive data may be exposed
- Requires strong access control

### Compliance Solutions
- Encryption
- Access control
- Audit logging
- Data governance policies

### Industry Example
E-commerce industry:
Customer data is loaded first, then transformed for reporting.

### Advantages
- Fast processing
- Highly scalable
- Flexible

### Disadvantages
- Compliance risks if not managed properly


## EtLT (Extract, Transform-lite, Load, Transform)
EtLT is a hybrid model combining ETL and ELT.
1. Extract data
2. Perform light transformation
3. Load data
4. Perform full transformation

### Process Flow
Source → Extract → Transform-lite → Load → Transform

### Compliance Benefits
- Early masking of sensitive data
- Flexible transformation
- Balanced performance

### Industry Example
Banking industry - Sensitive transaction data is partially masked before loading.

### Advantages
- Balanced performance
- Good compliance support

### Disadvantages
- More complex architecture