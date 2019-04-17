### Serveless -  Why can't we have best of bothe world (serverless and spring boot based api)

Looking into , how we can utilise the serverless apis(AWS Lambda with API Gateway)   in conjunstion with docker based application to manage transaction driven application to reduce the operating cost. Idea is to operate production grade application under 

- Looking at dashboard /client portal ( serveless api)
- Clinet Request (Order /applicaitons)
- Looking at operation requires proper transaction bounderies (spring boot app  )
- File based operation ( AWS sftp ,S3, ECS Task based on spring boot app running ECS Fargate ? / spot instance). most of the    transactional application stil requir interface with some sort of file to get some information. 
- Report generation (S3 ECS Task based on spring boot app ? or we have lightweight solution)
- use s3 as you key/value store (really cheap and highly scaleable )
- cost saving coming from serveless api and using tasks (no need to run servers 24s ). both scale infinitly . 
- set up will always run in multi region   diverting  client facing traffic  10/80 . 
- NOTE:dont have solution yet for bank end process (not every thing can be run simultaniously in diffrent region like file processing) which can run in diffrent regions like clinet facing portal 

- we will calculate the cost for each componenet and get rugh operating cost.

#### NOTE: This is not going to be production app for certain business use case. its just application to explore how we can reduce cost and increase availability. feature request are well come to reflect use cases out there.

#### if you want to contribute and have discussion around the project please create pull request to this page. Thanks !



