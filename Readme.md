## 14/MAY FRI
- DLV-11 global config service
  - build/deploy pipeline
    - problem solved (Runtime.ImportModuleError)
    - upload the zip file to s3
    - update lambda function
  - create PR
  - create Tech Debt tickets around Redis and ECR

## 13/MAY THU
- DLV-11 global config service
  - build/deploy pipeline
    - update bitbucket pipeline & shell scripts
    - Problem: Runtime.ImportModuleError: Error: Cannot find module 'aws-xray-sdk-core/lib/middleware/sampling/service_connector'
  - TODO:
    - Redis(Cache)

## 12/MAY WED
- DLV-11 global config service
  - jest test
  - build/deploy pipeline
  - TODO:
    - Redis(Cache)

## 11/MAY TUE
- DLV-11 global config service
  - deployed to poc account (for frontend testing) - used to get a trouble of cors.. add cors in express
  - solve the problem on redirecting root -> returning 404 on not ending with html
    - resolve: trailing slash set to true.
      - trailing slash false: p.html generated when it's built
      - trailing slash true: p/index.html generated when it's built

## 10/MAY MON
- DLV-11 global config service
  - use https://www.npmjs.com/package/@vendia/serverless-express as RMF
    - it makes us to reuse the framework we used already in the other serivce.
    - the existing framework already cover error handling, input validation and swagger

------------

## 07/MAY FRI
- DLV-11 global config service
  - solved CORS problem: the doc created (https://confluence.aurion.io/display/TDS/CORS+cases)
  - discussed to update UI, api and dynamodb: the doc updated (https://confluence.aurion.io/display/TDS/Global+Config)
  - update api super/(list|update)
  - RMF (Route Management Framework) (ATM, if/else)
    https://confluence.aurion.io/display/TDS/RMF+for+lambda+and+node.js

## 06/MAY THU
- DLV-11 global config service
  - update the dynamodb design and api spec following the discussion with Lea, Dan
  - implement api super/(list|create|update)
  - TODO:

## 05/MAY WED
- DLV-11 global config service
  - config/list with dynamodb mapper - deploy with node_module
  - dynamodb design? keys = MSCB, SGP
    - sk? incomeYear?
    - to query, pk is essential so query many times.
    - a record has one value but the attribute name is different depending on the PK
## 04/MAY TUE
- DLV-11 global config service
  - created lambda: { name: t50-global-config } function and linked to api-gateway
  - reviewed the global config api spec
  - add deploy procedure to lambda
  - build local test environment

## 03/MAY MON (HOLIDAY)

------------
## 30/APR FRI
- global config service
  - building test env.
    - lambda: { name: joung-test-app }
    - api-gateway: { name: joung-test-api }
    - loadbalancer: {
        name: joung-test-lb
        target-group: {
          name: joung-target-group
        },
      }

## 29/APR THU
- next.js
  - discuss the problem next.js trying to generate the route/page against the test files.
    - result: source code file name
  - fix eslint
  - merged
## 28/APR WED
- next.js
  - shared what I've changed to the team
  - Problem: next.js is trying to generate the route/page against the test files.
    - solve: source code file name 
## 27/APR TUE
- next.js
  - jest-ed (re-done a bit because pages updated by re-usable input)
  - TODO:
    - fix error on reusuable input
    - build pipeline

## 26/APR MON (HOLIDAY)

------------

## 23/APR FRI
- next.js
  - jest: mock next/router
  - problem: next.js is trying to build all files in pages including test files.
    - easiest: put test folder out of pages folder
    - solved: add ignore pattern into webpack config in next.config.js

## 22/APR THU
- next.js
  - image in storybook: just put them to public of next.js project
  - jest: access the components in storybook

## 21/APR WED
- next.js
  - pageContainer
  - pages:
    - done: all payroll admin and all employee
    - done: on board
    - done: updatepassword
## 20/APR TUE
- next.js
  - add _app.tsx which means configuration, theme and auth(login, user info)
  - pages:
    - done: login, forgot password
    - done: index/main -> redirect the page depending on the role.

## 19/APR MON
- next.js
  - build success in nerna and rush

------------

## 16/APR FRI
- next.js
  - coverting react.js to next.js
  - build failure when the component is out of the project.
## 15/APR THU
- next.js
  - read docs about deployment 

## 14/APR WED
- next.js
  - read docs about deployment

## 13/APR TUE
- T50-156 Button style
  - merged
- next.js
  - read docs
## 12/APR MON
- T50-156 Button style
  - done

------------

## 07/APR WED ~ 09/APR FRI (Annual Leave)

## 06/MAR TUE
- T50-156 Button style
  - the padding of the legend: 4px (default: 5px)
  - why I am doing this: Material Design and Material UI library are a little bit different.

## 05/APR MON (HOLIDAY)

------------

## 02/APR FRI (HOLIDAY)

## 01/APR THU
- T50-156 Button style
  - found the way how TextField has icons
  - update storybook textfield componnent

## 31/MAR WED
- T50-156 Button style
  - got feeback of the spacing before and after the label on the outlined TextField
  - found the build error on the pipeline
    - reason: the restriction on AWS user for deploying
    - solov: use a different user

## 30/MAR TUE
- T50-156 Button style
  - update Textfield style (override theme)
  - deploy Storybook

## 29/MAR MON (begin 3days lockdown)
- workshop
- discussion of Carl's configure driven mui component
- T50-156 Button style
  - update button style (override theme)

------------
## 26/MAR FRI
- T50-161 Investigate ORM
  - shared
- T50-156 Button style
  - investigating

## 25/MAR THU
- T50-161 Investigate ORM
  - (TypeORM) add index, more relation, transaction, logging

## 24/MAR WED
- T50-161 Investigate ORM
  - use TypeORM
    - run a normal query
    - connection with schema, find, save

## 23/MAR TUE
- T50-161 Investigate ORM
  - tried Sequelize

## 22/MAR MON
- T50-161 Investigate ORM
  - DynamoDB mapper for Tenant Config
    - new Tenant
    - get TenantConfigs

------------

## 19/MAR FRI
- T50-136 Design refinement - Login
  - done: to QA
- T50-138 UI Debt - Create a person
  - done: to QA
- T50-160 UI Debt - Employee Portal
  - done: to QA

## 18/MAR THU
- Tried to create Button/Textfield components in storybook-ui
  - needs more time.. created a new task for that

## 17/MAR WED
- Design refinement
  - TextField & PasswrodField with theme nesting
    - have a different primary color
  - Button with theme nesting
    - diabled color is different button variant

## 16/MAR TUE
- Design refinement
  - Login
    - OutlinedTextField having dark shaded primary colour
    - add PasswordBox into Storybook

## 15/MAR MON
- Design refinement
  - Login
    - add custom color to pallete
    - investigate Material System
      - especially color system

------------

## 12/MAR FRI
- Design refinement
  - Login
    - add LoginContainerUI into Storybook
    - use it on frontend-web

## 11/MAR THU
- T50-120 Run A Simple Pay
  - T50-2 Generate and Send Payslip Notification
    - done
- Design refinement
  - Login

## 10/MAR WED
- T50-120 Run A Simple Pay
  - T50-2 Generate and Send Payslip Notification
    - back-end payroll done
    - frontend-web almost done

## 9/MAR TUE
- T50-120 Run A Simple Pay
  - T50-9 snackbar aba
    - 3 amigos
    - DONE
  - T50-144 snackbar payslips
    - 3 amigos
    - DONE
  - T50-2 Generate and Send Payslip Notification
    - 3 amigos
    - make Payroll service have same basic configuration to Organisation service
    - doing

## 8/MAR MON
- T50-39 Employee Payslip
  - T50-8 access to payslip
    - Jest done
  - T50-11 payslip download
    - done

------------

## 5/MAR FRI
- T50-39 Employee Payslip
  - T50-8 access to payslip
    - Dev done

## 4/MAR THU
- T50-120 Run A Simple Pay
  - T50-15 aba
    - done
    - bugfix on build-mode to get object (Amplify.Storage was null)
- T50-39 Employee Payslip
  - T50-8 access to payslip
    - 3 amigos

## 3/MAR WED
- set-up Mac
- bug fix on connecting config api (Carl's change)
- T50-120 Run A Simple Pay
  - T50-15 aba
    - investigate s3 secure

## 2/MAR TUE
- T50-120 Run A Simple Pay
  - T50-15 aba
    - investigate s3 secure

## 1/MAR MON
- T50-120 Run A Simple Pay
  - T50-15 aba
    - 3 amigos
    - investigate s3 secure
  - T50-13 pay summary
    - fix build error in aws codebuild
      - increase node memory

------------

## 26/FEB FRI
- T50-120 Run A Simple Pay
  - T50-13 pay summary
    - export pdf

## 25/FEB THU
- T50-120 Run A Simple Pay
  - T50-13 pay summary
    - 3 amigos
    - table done

## 24/FEB WED
- T50-120 Run A Simple Pay
  - T50-19 add payrun spinner
    - done
- fix cicd problem

## 23/FEB TUE
- T50-120 Run A Simple Pay
  - T50-16 Conduct a payrun
    - jest
    - service: add status into Employee object
    - show only committed member on pay-run page
- fix pipeline problem making CORS in org service

## 22/FEB MON
- t50-120 create a person
  - T50-118 Create and Store
    - Merged
    - TODO: update status
- T50-120 Run A Simple Pay
  - T50-16 Conduct a payrun
    - UI thing & got some feedback from Jen
- some code reviews
  - build/docker.. -> update buildspec for cicd

------------

## 19/FEB FRI
- t50-120 create a person
  - T50-118 Create and Store
    - fix build error
    - add function to add group to the user
- T50-120 Run A Simple Pay
  - T50-16 Conduct a payrun
    - 3 amogos
    - UI thing

## 18/FEB THU
- t50-120 create a person
  - T50-118 Create and Store
    - call api via api-gateway
    - update design on Jen's comment

## 17/FEB WED
- t50-120 create a person
  - T50-118 Create and Store
    - Deploy testing environment in Lab account
	- org-service merged
	- TODO: 
    - call api via api-gateway
    - Update design on Jen's comment

## 16/FEB TUE
- t50-120 create a person
  - T50-118 Create and Store
	- cors in backend
	- create employee api call
	- snackbar / notistack
    - creating ConfigProvider
	- jest
	- TODO: Update design on Jen's comment
			Test in aws ecs

## 15/FEB MON
- t50-120 create a person
  - T50-118 Create and Store
    - test codes: done
    - back to frontend
    - creating config context
- TTN-4733 QSS 500 Errors
  - sign-off

------------

## 12/FEB FRI
- t50-120 create a person
  - T50-118 Create and Store
    - employee service: done (get, list, create and delete)
    - jest: env and db connect: done (mock process.env, aws secret manager)
  * TODO
    - jest: employee (mock db)

## 11/FEB THU
- t50-120 create a person
  - T50-118 Create and Store
    - build pipeline
    - eslint configuration
    - fix the jest configuration by Carl
    - create employee normal process done
  * TODO
    - check the api path to Lea
    - test case
  - t50-7 navigation
    - fix the bug on test
    - change label and url path

## 10/FEB WED
- t50-120 create a person
  - T50-118 Create and Store
    - understand the backend architecture from Lea
    - get the sample code and postman collection
    - connect to the database in lab accout
    - initialize organisation-service (copy from payroll-service)
    - jest configuration (babel, typescript)
    - how to mock postgresql: https://stackoverflow.com/questions/59540432/how-to-mock-postgresql-pg-in-node-js-using-jest
  * TODO
    - write unit test code
    - add environment variables into fargate (aws credential - only for POC)
      - Go to Task Definition on ECS and create new revision
  - t50-7 navigation
    - code review: updated
  - t50-117 Data input
    - comes along with t50-7

## 09/FEB TUE
- t50-120 create a person
  - t50-7 navigation
    - deved screen and test
    - deployeed to http://dwqnootvjrgl8.cloudfront.net/
    - Merge request

## 08/FEB MON
- t50-6 login
  - code reviewed
  - go back to the previous page after login
  - #TODO: f5, redirect to root when logged-in user visits login page
- t50-120 create a person
  - t50-7 navigation
    - test codes

------------

## 06/FEB SAT
- t50-6 login
  - jest unit test: almost 100% coverage

## 05/FEB FRI
- t50-6 login
  - CloudFront config fix: add error page (404 -> index.html & 200)
  - Config API (including CORS)
  - jest unit test: make it correct & better coverage

## 04/FEB THU
- t50-6 login
  - error message for wrong password
  - caps lock message
  - add jest unit test (just coverage > 80%)

## 03/FEB WED
- t50-6 login
  - update the design against Jen's feedback
  - TODO: 1)Config API, 2)error message for wrong password, 3)caps lock message
- BELT
  - bugfix when core.verion is null

## 02/FEB TUE
- t50-6 login
  - pull Carl's changes around authprovide & update to use cognito api
  - update the design
  - TODO: form validation, catch up the feedback from Jen
- BELT
  - investigate the crash
## 01/FEB MON
- t50-6 login
  - ForgotPassword: logic done.
    - use code, not link (workflow's changed)
    - new password: url access -> a part of Forgot password
  - TODO: form validation
  - TODO: enhance authprovider with Carl

------------

## 29/JAN FRI
- t50-6 login
  - Login, Forgot-password, New-password pages: ui done.
    - all pages have the same layout
    - password box having show/hide icon: done
  - merged from Carl's router code
  - TODO: in firefox, the layout is different.
  - TODO: enhance authprovider, give url-route to forgotpassword and newpassword

## 28/JAN THU
- t50-6 login
  - use auth api manually: ** almost done
  - Login page
  

## 27/JAN WED
- t50-6 login
  - hard to customize login UI when using pre-built amplify react components
  - use auth api manually: ** ing
(Interview James Nguyen)

## 26/JAN TUE: Australian Day

## 25/JAN MON
- T50POC: add buildspec for payroll service  
- t50-6 login
  - inherit SigIn class from aws-amplify-react
  - import material ui for the component.
  - dev.ing password component

------------

## 22/JAN FRI
- T50
  - backend infrastructure: apigw: ** done

## 21/JAN THU
- T50
  - backend infrastructure: ecr, vpc - ecs (cluster - service) : ** done

## 20/JAN WED
- T50
  - Create a new project for codepipeline cdk
  - figured how to disable the default pipeline trigger
  - MR for frontend buildpipeline to t50poc-pipeline project
    - add cicd stack (repository, lambda pipeline trigger, codebuild, codepipeline for frontend)
  - MR for frontend buildpipeline to t50poc project
    - add buildspec file
  - start backend infrastructure

## 19/JAN TUE
- T50
  - Codebuild on Lab can access Nexus server. (using Nexus VPC)
  - Customizing triggers for AWS CodePipeline with AWS Lambda and Amazon CloudWatch Events

## 18/JAN MON
- T50
  - build cdk pipeline for t50poc
  - create user for gitlab to mirror
    id: t50-gitlab
    pw: ~.;vyw3s@MMtBgc
  - git credential
    t50-gitlab-at-406353380800
    09lNwpWfBi/xHsWAM9lPPrJaXtmJu7kJrBqP3sY3rL8=
  - mirror (gitlab -> codecommit) ==> done
  - ** lab account cannot access to nexus: waiting for Al
  - ** Multiple pipelines with a single source to support monorepos

------------

## 15/JAN FRI
- T50
  - build pipeline using gitlab
  - session from Stanley about aws pipeline

## 14/JAN THU
- T50
  - cdk for web application


## 13/JAN WED
- T50

## 12/JAN TUE
- T50


## 11/JAN MON
- TTN-4678 Change Message Server to a manual start service
  - signup & merged

- TTN-4733 QSS 500 Errors
  - TTN-4758 [low] Shut session-file-store up. Again.
    - get Carl's comment and reply with a new code

- T50
  - Architecture Review
  - Mono/Multi Repo Review
  - build cicd for frontend
	https://medium.com/@trevlinp/react-continuous-deployment-with-gitlab-ci-and-s3-46987e30dc54
