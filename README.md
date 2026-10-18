### Tapuwanashe Magumise

Cloud engineer in Harare, Zimbabwe. AWS Certified Solutions Architect and Developer (Associate). I spent almost three years moving 9 hospitals off paper records and onto AWS, and I now run [PayCanary](https://paycanary.io), a risk monitoring product for Stripe merchants.

My portfolio site, with case studies of all nine projects and my CV: [tapiwa-magumise.github.io/portfolio](https://tapiwa-magumise.github.io/portfolio/)

Each project below has an architecture diagram, the design decisions with their trade-offs, and results measured by the code in the repo.

**Foundations and security**

| Project | What it shows |
|---|---|
| [Multi-Account Landing Zone](https://github.com/tapiwa-magumise/aws-landing-zone) | AWS Organizations in Terraform with service control policies, an organisation-wide CloudTrail under Object Lock, and IAM Identity Center sign-in |
| [Hybrid Migration and DR](https://github.com/tapiwa-magumise/aws-hybrid-migration-dr) | Office app, database and files moved to AWS with 94 seconds of frozen writes; back up in Ireland 18 min 27 s after London went down |
| [Security and Cost Review Agent](https://github.com/tapiwa-magumise/aws-security-cost-review) | Reviews Terraform or a live account against 24 Well-Architected rules through a read-only role |

**Data**

| Project | What it shows |
|---|---|
| [Serverless Sales Pipeline](https://github.com/tapiwa-magumise/aws-serverless-sales-pipeline) | S3, SQS, Lambda, DynamoDB and Athena; every row validated and every file audited; deployed with OIDC, no stored keys |
| [Edge Analytics](https://github.com/tapiwa-magumise/aws-edge-analytics) | CloudFront logs turned into CDN cost by region, page speed, A/B results and bot traffic with Step Functions, Glue and Athena |
| [Online Retail Analytics](https://github.com/tapiwa-magumise/retail-analysis-case-study) | 1,067,371 transactions analysed in DuckDB and Python, reported in Power BI |

**Applications**

| Project | What it shows |
|---|---|
| [Invoicing and Payments API](https://github.com/tapiwa-magumise/invoicing-api) | FastAPI, PostgreSQL and Redis; a retried payment never charges twice; 10,734 requests with 0 errors under load |
| [Event-Driven Order System](https://github.com/tapiwa-magumise/event-driven-orders) | NestJS and Spring Boot over Kafka on Kubernetes; 40 orders raced for 10 items and exactly 10 went through |

**AI**

| Project | What it shows |
|---|---|
| [Governed RAG Assistant](https://github.com/tapiwa-magumise/governed-rag-assistant) | UK procurement answers from 260 documents on Amazon Bedrock in London, with citations, personal data masking and an ISO/IEC 42001 governance pack. Evaluation still to run |
