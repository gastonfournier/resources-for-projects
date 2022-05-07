This page tries to cover many aspects of choosing DynamoDB as the storage solution and tries to provide hints and guidance about the technology.

# Is it the right tool for you?

You have to consider many aspects which are described in [this post](https://aws.amazon.com/es/blogs/database/how-to-determine-if-amazon-dynamodb-is-appropriate-for-your-needs-and-then-plan-your-migration/), but overall, if you can’t predict your access patterns or are likely to change frequently, you need to run ad hoc queries on your data, then probably DynamoDB is not the best tool for you.

# Designing for NoSQL

You should clearly understand your relational schema (all data is relational), and starting from the relational model, denormalize it into one or two tables fulfilling your access patterns. Some resources to get started:
1. [Data modeling (part 1)](https://www.youtube.com/watch?v=fiP2e-g-r4g)
2. [Data modeling (part 2)](https://www.youtube.com/watch?v=0uLF1tjI_BI)
3. [Advanced design patterns (part 1)](https://www.youtube.com/watch?v=MF9a1UNOAQo)
4. [Advanced design patterns (part 2)](https://www.youtube.com/watch?v=_KNrRdWD25M)
5. [The What, Why, and When of Single-Table Design](https://www.alexdebrie.com/posts/dynamodb-single-table/)
6. [How DynamoDB scales where relational databases don't](https://www.alexdebrie.com/posts/dynamodb-no-bad-queries/)

# Examples of Modeling Relational Data in DynamoDB
1. [Example of modeling relational data in DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/bp-modeling-nosql-B.html)
2. [Instagram model](https://docs.google.com/spreadsheets/d/1IWVXyiJ0y4DF6ii-H6vKCF0qQUZr4akI59IaiL1ArIs/edit#gid=1488945379) from Alex DeBrie, with code https://github.com/alexdebrie/dynamodb-instagram#readme"


# Dive deep
1. https://github.com/papers-we-love/papers-we-love/blob/master/datastores/dynamo-amazons-highly-available-key-value-store.pdf
