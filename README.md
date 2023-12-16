# DE_ELT_Retail
Data Engineer Project for TPC-H Retail Data using snowflake as cloud warehouse and dbt (data build tool) as transformation framework for an ELT pipeline

## Pipeline Architecture
![2c5c42d3c339b6b9](https://github.com/AbdiasPC/DE_ELT_Retail/assets/48920867/82adc6d0-e5eb-4c31-a5cf-445c53c03b73)

## Sample Data: TPC-H
TPC-H is a decision support benchmark. It consists of a suite of business-oriented ad hoc queries and concurrent data modifications. The queries and the data populating the database have been chosen to have broad industry-wide relevance. This benchmark illustrates decision support systems that examine large volumes of data, execute queries with a high degree of complexity, and give answers to critical business questions.

### Database and Schemas
TPC-H comes with various data set sizes to test different scaling factors. For demonstration purposes, we’ve shared four versions of the TPC-H data. The data is provided in the following schemas in the SNOWFLAKE_SAMPLE_DATA shared database:

* TPCH_SF1: Consists of the base row size (several million elements).
* TPCH_SF10: Consists of the base row size x 10.
* TPCH_SF100: Consists of the base row size x 100 (several hundred million elements).
* TPCH_SF1000: Consists of the base row size x 1000 (several billion elements).

### Database Entities, Relationships, and Characteristics

The components of TPC-H consist of eight separate and individual tables (the Base Tables). The relationships between columns in these tables are illustrated in the following ER diagram:
<img width="615" alt="sample-data-tpch-schema" src="https://github.com/AbdiasPC/DE_ELT_Retail/assets/48920867/283feb39-e3e4-47c0-9112-6a9652dd6d96">
