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
