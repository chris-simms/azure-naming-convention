# Azure Naming Convention

| #   | Tag Key       | Required? | Description                                                | Example Value(s)             |
| :-- | :------------ | :-------- | :--------------------------------------------------------- | :--------------------------- |
| 1   | business_unit | Yes       | Logical group of products for cost managment               | technology, marketing, sales |
| 2   | environment   | Yes       | Deployment iteration of a product                          | test, dev, qa, uat, prod     |
| 3   | product       | Yes       | Application, service, or workload within the business unit | sysops, networking, o365     |
| 4   | component     | Yes       | Module of the product                                      | ansible, jira, excelapi      |
| 5   | function      | Yes       | Purpose or language of the component                       | automation, itsm, aspnet     |
| 6   | product_owner | Yes       | Person responsible for approving costs for the product     | satya_nadella, phil_spencer  |

## Tag Hierarchy
- business_unit
  - environment
    - product
      - product_owner
      - component
        - function
