## 08/JAN FRI
- DRM-1007 Update Dependency to pass yarn audit
  - rollback PR ready

- TTN-4678 Change Message Server to a manual start service
  - bugfix: when enable/disable env and service is not running... not set Start-up type

## 07/JAN THU
- DRM-1007 Update Dependency to pass yarn audit
  - nextus upload setup

## 06/JAN WED
- DRM-1007 Update Dependency to pass yarn audit
  - re-generate the build fail issue


## 05/JAN TUE
- TTN-4733 QSS 500 Errors
  - TTN-4758 [low] Shut session-file-store up. Again.
- DRM-1007 Update Dependency to pass yarn audit
  - axios version up https://www.npmjs.com/advisories/1594
- TTN-4666 new spin list survey answer type
  - reviewing


------------

# 2020

------------

## 18/DEC FRI
- TTN-4733 QSS 500 Errors
  - TTN-4760 [low] remove stack traces for soft errors
  
## 17/DEC THU
- TTN-4733 QSS 500 Errors
  - TTN-4760 [low] remove stack traces for soft errors

## 16/DEC WED
- TTN-4733 QSS 500 Errors
  - TTN-4758 [low] Shut session-file-store up. Again.
  - TTN-4760 [low] remove stack traces for soft errors

## 15/DEC TUE
- TTN-4678 Change Message Server to a manual start service
  - TTN-4711 2. Add button to start/stop Message Service
    decide to use the original button style
    done & reviewed
  - TTN-4713 4. Change the apply process order of "start Message Service"
    done & reviewed
- t50
  - reading miro

## 14/DEC MON
- TTN-4678 Change Message Server to a manual start service
  - TTN-4711 2. Add button to start/stop Message Service
    - implementing button style
	- old version doesn't supoort trigger override

------------

## 11/DEC FRI
- TTN-4678 Change Message Server to a manual start service
  - TTN-4711 2. Add button to start/stop Message Service
    - discuss button style
    - background logic: done

## 10/DEC THU
- TTN-4678 Change Message Server to a manual start service
  - TTN-4710 1. Add toggle button Message Service start option "manual/auto"
    - found bug - fixed
	- reviewing
	- pending test
  - TTN-4711 2. Add button to start/stop Message Service
    - discuss button style
  
## 9/DEC WED
- TTN-4678 Change Message Server to a manual start service
  - TTN-4710 1. Add toggle button Message Service start option "manual/auto"
    - found bug: do not delete MsgServerServiceName field
  - TTN-4711 2. Add button to start/stop Message Service
    - discuss button style
	- add backgroud worker for watching service running

## 8/DEC TUE
- TTN-4678 Change Message Server to a manual start service
  - TTN-4711 2. Add button to start/stop Message Service

## 7/DEC MON
- TTN-4678 Change Message Server to a manual start service
  - TTN-4710 1. Add toggle button Message Service start option "manual/auto"
    - when upgrade BELT, set auto as startup type for existing environment using msg-server
	- reviewing

------------

## 4/DEC FRI
- TTN-4678 Change Message Server to a manual start service
  - TTN-4710 1. Add toggle button Message Service start option "manual/auto"
    - refactoring msg server/checker
	- visibility of start option
  
## 3/DEC THU
- TTN-4678 Change Message Server to a manual start service
  - decision: no shotcut (discussed w/ Carl, Ash)
  - TTN-4710 1. Add toggle button Message Service start option "manual/auto"
    - ing. hide A/M button when core version is old (less than 11.72)
  
## 2/DEC WED
- TTN-4678 Change Message Server to a manual start service
  - collaboration - done
  - TTN-4710 1. Add toggle button Message Service start option "manual/auto"
    -

## 1/DEC TUE
- TTN-4678 Change Message Server to a manual start service
  - discussed w/ Ash, Jules
  - create the cmd batch file to toggle it
  - with Cam... 3 toggle buttons: 1) install, 2) start automatically or manually, 3) turn it on/off without Apply environment

- TTN-4706 Email link to ESS reports gives error 500 (ARN-42876)
  - SAML error is not a reason of 500
  - 500 should show UUID but tech team override 500 page so cannot get UUID
  - ask Jake to ask the Customer to try something

## 30/Nov MON
- BDD cucumber for Jira
  - living documentation: build ci for branching
  - demo
  
- TTN-4678 Change Message Server to a manual start service
  - discussed w/ Ash, Jules
  - create the cmd batch file to toggle it
  - with Cam... 3 toggle buttons: 1) install, 2) start automatically or manually, 3) turn it on/off without Apply environment

------------

## 27/Nov FRI
- BDD cucumber for Jira
  - living documentation: build ci (automatically upload the test result)

- TTN-4678 Change Message Server to a manual start service
 
- ARN-42876 Email link to ESS reports gives error 500
  - investigated w/ Ash, Jules
  - ask asn to Nick

- TTN-4604 Move the Message Service starting phase towards end of the apply
  - Cancelled & move to TTN-4678

## 26/Nov THU
- BDD cucumber for Jira
  - cucumber.js result json file format: cucumber-js --format=json > result.json
  - upload result file manually -> status shown

- TTN-4604 Move the Message Service starting phase towards end of the apply
  - problem: couldn't start message server service on 11.73.0.1
  - reproduce:
    1. create 11.73.0.1 environment with (old) t-shirt (without msg-server)
	1. set msg-server on, and apply, then error happens.

- TTN-2235 Remember Training Course Search Results
  - sign-off

## 25/Nov WED
- BDD
  - cucumber.js report
- TTN-2235 Remember Training Course Search Results
  - testing
- TTN-4604 Move the Message Service starting phase towards end of the apply
  - read/investigate codes
    appy button click -> OnApplyChangesCommand -> GenerateApplyJobs

GenerateApplyJobs
## 24/Nov TUE
- TTN-2235 Remember Training Course Search Results
  - type: flatpickr
  - reviewing
- BDD
  - cucumber.js tutorial
  - link to living document (cucumber for Jira)
  
## 23/Nov MON
- TTN-2235 Remember Training Course Search Results
  - type: flatpickr
  - ie11 doesn't support FormData fully. - move to

------------


## 20/Nov FRI
- TTN-2235 Remember Training Course Search Results
  - convert to typescript
  - type: datatable.net, tablelist, loading

## 19/Nov THU
- TTN-2235 Remember Training Course Search Results
  - bugfix on IE11

## 18/Nov WED
- TTN-2235 Remember Training Course Search Results
  - Unit test: match the snapshot having empty csrf input field
  - urijs
  - hide the core field names

## 17/Nov TUE
- TTN-2235 Remember Training Course Search Results
  - review feedback
    - Unit test for cache-control & csrf
    - urijs
    - hide the core field names
  - Unit test for cache-control: done

## 16/Nov MON
- TTN-2235 Remember Training Course Search Results
  - TTN-4664 3. Restore page state when return to page
    - restores table resulte from session storage
	- restores table page
	- restoring search conditions (autocomplete, date picker)

------------

## 13/Nov FRI
- TTN-2235 Remember Training Course Search Results
  - TTN-4663 2. Cache search results and page state in SessionStorage
    - no needs random key because tab has a separated session storage-with-amazon-dynamodb/
	- get page and save it.
    - dev: done, review: done, testing

## 12/Nov THU
- TTN-2235 Remember Training Course Search Results
  - TTN-4663 2. Cache search results and page state in SessionStorage
	- random key
    - datatable page

## 11/Nov WED
- TTN-2235 Remember Training Course Search Results
  - TTN-4662 1. Allow browser to cache page & search AJAX method change
    - dev done, review done, testing
  - TTN-4663 2. Cache search results and page state in SessionStorage
	- replace url(state) done
    - save & load table body: done
	- window.history.state?

## 10/Nov TUE
- TTN-2235 Remember Training Course Search Results
  - collaboration

## 9/Nov MON
- TTN-2235 Remember Training Course Search Results
  - investigating 304, csrf

------------

## 6/Nov FRI
- TTN-2235 Remember Training Course Search Results
  - investigating 304, etag, csrf

## 5/Nov THU
- TTN-2235 Remember Training Course Search Results
  - investigating

## 4/Nov WED
- TTN-4059 AutoSave
  - Sign off
- TTN-2235 Remember Training Course Search Results
  - investigating

## 3/Nov TUE
- TTN-4059 AutoSave
  - TTN-4513 Handle Edge cases
    - QA done
- TTN-2235 Remember Training Course Search Results
  - investigating 304
    - cache-control, etag, if-none-match, pragma

## 2/Nov MON
- TTN-4059 AutoSave
  - Handle the error not relating invalid inputs
    should not show auto-saved notification as well as error message
  - unit test

------------

## 30/Oct FRI
- TTN-4059 AutoSave
  - notification behaviour
    - no progress bar on top
	- AUTO-SAVE after saved
	- nothing during saving

## 29/Oct THU
- TTN-4059 AutoSave
  - 2 seconds minimum notification show time
  - waiting Cam and Jenny
- BDD

## 28/Oct WED
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
    - QA testing
	- deploy via ngrok, so Cam and Jenny can travel.
    - fix the bug on the radio table
  - TTN-4513 Handle Edge cases
    - PerformanceHistory, PerformanceForm and ApplicationFormController: add routes and work well
	- RefereesController, ReviewApplicantsController and InterviewsController work well

## 27/Oct TUE
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
    - reviewed
  - TTN-4513 Handle Edge cases
    - investigating: https://jira.aurion.io/browse/TTN-4513?focusedCommentId=87265&page=com.atlassian.jira.plugin.system.issuetabpanels:comment-tabpanel#comment-87265

## 26/Oct MON
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
	- bugfix on insert/delete row with invalid value
	- Emit an event when modal opens
	
------------
## 23/Oct FRI
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
    - bugfix on DateBox on Modal
	- bugfix-ing on insert/delete row with invalid value
	  : server side done 

## 22/Oct THU
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
    - Write the test scenario
    - bugfix on Date-Picker on Modal
    - bugfix on Select on Modal

## 21/Oct WED
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
    - bugfix on insert/remove row
	- avoid infinite loop
	
## 20/Oct TUE
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
    - bugfix-ing on insert/remove row
	
## 19/Oct MON
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
	- make the cancel button work properly

------------
## 16/Oct FRI
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
	- document attachment: done

## 15/Oct THU
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
    - codepicker: done
	- document attachment: doing

## 14/Oct WED
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
	- rollback the invalid value with old/good value --> implemented (Carl reviewed)
	- testing...

## 13/Oct TUE
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
    - auto-save logic change: auto save 30 sec later when they leave. (not every 30 secs)
	- try to remove the invalid column -> result: data cleared
	- rollback the invalid value with old/good value --> implementing

## 12/Oct MON
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
    - normal case: done
	- invalid value case: implementing


------------

## 09/Oct FRI
- TTN-4059 AutoSave
  - TTN-4512 Handle Tables
    - implementing

## 08/Oct THU
- TTN-4059 AutoSave
  - TTN-4511 Server Changes
    - Tested
  - TTN-4512 Handle Tables
    - notification for table modal: discussed from Jenny
	- investigation
	- design review from Carl

## 07/Oct WED
- TTN-4463 grooming
- TTN-4059 AutoSave
  - TTN-4511 Server Changes
    - reviewed

Raml-esque

## 06/Oct TUE
- TTN-4059 AutoSave
  - TTN-4511 Server Changes
- Core Competencies : Tax Calculation
  - https://helpcontent.aurion.com/11.74/core/Default.htm#HelpTopics/Pay/TaxNetPay/Calculating_PAYG_Tax.htm?Highlight=payg
  - https://www.ato.gov.au/rates/schedule-1---statement-of-formulas-for-calculating-amounts-to-be-withheld/
  - Tax Rates
  - Employee Tax and Net Pay Details
- TTN-4463 grooming

## 05/Oct MON Public Holiday


------------

## 02/Oct FRI
- TTN-4059 AutoSave
  - TTN-4511 Server Changes
    - save valid answers (iterate in node server side)
	- when save, reset auto-save

## 01/Oct THU
- TTN-4059 AutoSave
  - TTN-4511 Server Changes
    - reviewing
	- discuss about the invalid answers: not ignore, save the valid answers.
	- disable the buttons when auto-save
  - TTN-4512 Handle tables
    - implementing

## 30/Sep WED
- TTN-4059 AutoSave
  - TTN-4510 Client Changes
    - reviewing
	- Jules' comment: auto saving interval can be configurable
	- Cam's reply: not giving the option to configure
  - TTN-4511 Server Changes
    - implemented

## 29/Sep TUE
- TTN-4059 AutoSave
  - TTN-4510 Client Changes
    - implemented & reviewing

## 28/Sep MON
- TTN-4059 AutoSave
  - TTN-4509 Notification UI
    - Implement & reviewed
- Training: Culture Amp Performance
- BDD
  - added Xray

------------

## 25/Sep FRI
- TTN-4059 AutoSave
  - TTN-4514 Investigate
  - TTN-4509 Notification UI
    - discuss with Jenny

## 24/Sep THU
https://mobileapptest.aurion.io/DevTest/login
https://confluence.aurion.io/display/PROD/Internal+App+Test+Environment

## 23/Sep WED
- TTN-4100 Update Super instructions in Onboarding
  - sign-off
- TTN-4100 Update Super instructions in Onboarding
  - Learn survey
  - Collaboration

## 22/Sep TUE Annual leave

## 21/Sep MON Annual leave

------------

## 18/Sep F
- TTN-4059 AutoSave
  - Collaboration
    - user type & save at the same time
	- toggle function
	- status: timelapse
	- after-action saved or not saved
- TTN-4100 Update Super instructions in Onboarding
  - Collaboration
  - Source Code done
  - Pull Request
  - Reviewed
  - Waiting Test

## 17/Sep T
- Investigate Onboarding Login
  : https://confluence.aurion.io/pages/viewpage.action?pageId=85822011
- Estimate Web backlog: TTN-4059 TTN-4100
- TTN-4059 AutoSave
  - Investigate Paga & source code

## 16/Sep W
- Investigate Onboarding Login
- fix bug on jest config roots

## 15/Sep T
- Investigate Onboarding Login

OP008_ONBOARDING_LOGIN
EN020_GET_ONBOARDING_PORTAL

C:\ws\aurion-core\sources\components.dir\S_CONNECT_SEC.XML Line: 2118
  - OP008_ONBOARDING_LOGIN
C:\ws\aurion-core\sources\components.dir\S_CONNECT_SEC.XML Line: 154
  - EN030_GET_ALL_CANDIDATE_DETS
    - OP008_ONBOARDING_LOGIN

OP008_ONBOARDING_LOGIN (C:\ws\aurion-core\sources\components.dir\S_CONNECT_SEC.XML Line: 2033
 - retrieve/e "T320_WEB_CANDIDATE"
 - C:\ws\aurion-core\sources\components.dir\S_CONNECT_SEC.XML Line: 2117
 - EN030_GET_ALL_CANDIDATE_DETS (C:\ws\aurion-core\sources\components.dir\S_CONNECT_SEC.XML Line: 2125
                                (C:\ws\aurion-core\sources\components.dir\S_CONNECT_SEC.XML Line: 124
   - C:\ws\aurion-core\sources\components.dir\S_CONNECT_SEC.XML Line: 154
   
   
       if (!P_ACTIVATING)
        if (T320F025_STATUS != "R")
            P_MESSAGE = "Candidate with email address %%T320F010_EMAIL.T320_WEB_CANDIDATE%%% has not Registered" 140

## 14/Sep M
- Investigate Web Issues
  - https://jira.aurion.io/browse/TTN-4059 AutoSave
  - https://jira.aurion.io/browse/TTN-458 Mail Bulk-read-mark
  - https://jira.aurion.io/browse/TTN-4100 Update Super instructions in Onboarding
  - https://jira.aurion.io/browse/TTN-342 Hide message field
  - https://jira.aurion.io/browse/TTN-3196 SSO
  
------------

## 11/Sep F Office
- BDD
  - Jira BDD Tools

## 10/Sep T Office
- BDD
  - Jira BDD Tools

## 09/Sep W Office
- BDD
  - Jira BDD Tools

## 08/Sep T
- BDD
  - Jira BDD Tools

## 07/Sep M Office
- Trace the error when deleting account in recruitment.
  - because Bad Data
- Set up Core again.
- BDD
  - Jira BDD Tools

------------
  
## 04/Sep F Office
- TTN-4467 Restructure SEEK Credentials
  - done
- BDD

## 03/Sep T Office
- TTN-4338 register candidate
  - button on IE11
  - Merged to dev branch

## 02/Sep W
- TTN-4338 register candidate
  - bugfix on getting position data against vacancy key
  - button on IE11

## 01/Sep T
- investigate bluebird warning

## 31/Aug M
- password: 555Coronation
- TTN-4338 register candidate
  - the account which registred/applied with Seek cannot see the Questionnaire tab.... so cannot submit.

------------

## 28/Aug F
- TTN-4338 register candidate
  - bugfix: country code
  - bugfix: button size
  - Done... moving to TEST

## 27/Aug T
- TTN-4338 register candidate
  - pairing with Carl: refactoring SeekService.ts
  - update test code for refactoring

## 26/Aug W
- TTN-4420 mapping the country codes 11am
  - sign off
- BDD Research: Javascript BDD
  - https://confluence.aurion.io/display/OI/Javascript+BDD+tools

## 25/Aug T
- TTN-4338 register candidate
  - push & PR
  - solve the problem around `@types/express-handlebars`

## 24/Aug M
- TTN-4338 register candidate
  - unit test cases (to match snapshot using supertest, sinon)

------------

## 21/Aug F
- TTN-4338 register candidate
  - refactor SeekService.ts
  - unit test cases
    - 
- TTN-4440 Remove SEEK completion field from Web Candidate resume tab in 11.72
  * sign off

## 20/Aug T
- TTN-4338 register candidate
  - base64url & its test cases.
  - new Custom Error for seek & expired page shown only if error is invalid_grant
     ... others: show the error
  - refactor SaveFile, SaveModel w/Params
  - add SeekCodeExpired to login
  - add ADDRESS_SOURCE to AS037_WCSECURITY.OP001_WC_SIGNIN
  - refactoring ... some....
  
## 19/Aug W
- TTN-4338 register candidate
  - save the file before login
  - get/update the resume request key before login

## 18/Aug T
- TTN-4338 register candidate
  - signup complete
  - pairing

## 17/Aug M
- TTN-4338 register candidate
  - fill the signup form
  - raise 2 issues
    1. cannot upload the file before login
	1. ADDRESS_SOURCE for signup

------------

## 14/Aug F : Ekka public holiday

## 13/Aug T
- TTN-4420 country code
  : Created PR -> Reviewing
- TTN-4338 register candidate
  : keep going
  : redirection
  
## 12/Aug W
- TTN-4420 country code
  : implement a new logic
- setup Core in local
- TTN-4440 Remove SEEK completion field from Web Candidate resume tab in 11.72

## 11/Aug T
- TTN-4338 register candidate
- TTN-4420 country code
  : a new logic by John and Carl
  : delete old logic

## 10/Aug M
- TTN-4338 register candidate
  - create the sub-tasks & move to wip
  - seek code expired page -> sentense & design -> Jenny
  - modify process to handle expired seek code
- Dreampay result (9:30 - 11am)
- Aurion townhall (11am - 12pm)

------------

## 7/Aug F
- TTN-4338 register candidate
  - collaboration
  - new page for seek code expired

## 6/Aug T
- TTN-4420 country code
  - pushed
  - set local core environment
- TTN-4338 register candidate
  - read the tech note Carl & John discussed

## 5/Aug W
- TTN-4341 call complete link to SEEK
  - PR: approved. moved to test
- TTN-4338 register candidate
  - Collaboration
- TTN-4420 country code
  - try the rule for AU and NZ
- BDD: CucumberStudio for Jira: Hiptest

## 4/Aug T
- TTN-4341 call complete link to SEEK
  - unit test
  - PR
- TTN-4338 register candidate
  - review the requirement
- BDD: CucumberStudio for Jira

## 3/Aug M
- TTN-4341 call complete link to SEEK
  - impl: 2 seek apis
    1. get access token grant type is client_credentials
    2. call complete link 
- TTN-4339
  - Test completed, source code merged

------------

## 31/Jul F
- TTN-4341 Update "application submitted" page to mark SEEK application as completed
  - review the requirement
  - collaboration: Carl & Chris
- BDD: investigation from Jira & jest

## 30/Jul T
- TTN-4339
  - jest unit test case for SeekApi
  - trimming to max length
- TTN-4339/TTN-4391 Save personal details and completion link against application record
  - save complete link

## 29/Jul W
- TTN-4339/TTN-4392 Download resume and save to core
  - address input test: AU from SEEK, Australia
  - PR: got some comments and fix them. and discussion with Carl.

## 28/Jul T
- TTN-4339/TTN-4392 Download resume and save to core
  - tide the code up
  - Add exception handling
  - Add test case
  - how to input address to SEEK?

## 27/Jul M
- TTN-4339/TTN-4392 Download resume and save to core
  -(works functionally)
  - Download resume from SEEK
  - Save to core
    - add function to create the application record.

------------

## 24/Jul F
- TTN-4339/TTN-4390,4391 Save personal details and completion link against application record
  - TDD: test code
  - phone number validate
- retro
  hold back

## 23/Jul T   
- TTN-4339/TTN-4390,4391 Save personal details and completion link against application record
  - got reviewed and comments: fix them
  - code together with Carl (3 hours): code tidy up, TDD

## 22/Jul W
- TTN-4390 download person's details from SEEK
- TTN-4391 Save personal details and completion link against application record
  - draft, almost done
  
## 21/Jul T
- TTN-4389 Research: How Vacancy application form code and process works
  - Save document: https://confluence.aurion.io/display/~JoungPark/Save+document

## 20/Jul M
- TTN-4389 Research: How Vacancy application form code and process works
  - Edit candidate personal: https://confluence.aurion.io/display/~JoungPark/Edit+candidate+personal

------------

## 17/Jul F
- TTN-4389 Research: How Vacancy application form code and process works
  - other tabs and pages https://confluence.aurion.io/display/~JoungPark/Unclassified
- BDD
  - Angular .spec.ts and Jasmine: https://confluence.aurion.io/display/OI/Angular+spec.ts%3A+but%2C+more+about+Jasmine
ACP: Aurion Cloud Platform

## 16/Jul T
- TTN-4389 Research: How Vacancy application form code and process works
  - How the application page works: https://confluence.aurion.io/display/~JoungPark/How+the+application+page+works

## 15/Jul W
- TTN-4389 Research: How Vacancy application form code and process works
  - How to get data from Core: https://confluence.aurion.io/display/~JoungPark/How+to+get+data+from+Core
  - How the application page works: https://confluence.aurion.io/display/~JoungPark/How+the+application+page+works

## 14/Jul T
- TTN-4389 Research: How Vacancy application form code and process works
  - Start from packages/web/app.js: https://confluence.aurion.io/pages/viewpage.action?pageId=88672363

## 13/Jul M
- Read the web code
- Pre TTN-4337
  - GET credential from Core
  - Exchange access code with auth code
  - Get profile from SEEK

------------

## 10/Jul F
- Read the web code
- On-SEEK process: no auth code

## 09/Jul T
- Test On-SEEK process
  - JW fixed: /vacancy/{vacancyId}
  - My suggestion: /apply/{vacancyId}/apply
- Read the web code
  
## 08/Jul W
- TTN-4335 Update vacancy application page
  - test from the result of TTN-4336

## 07/Jul T
- TTN-4335 Update vacancy application page
  - merged to dev branch
  - move to test with how to test document
- aurion-web investigation
  - html -> core

## 06/Jul M
- TTN-4335 Update vacancy application page
  - got comments from Carl and fix them
- aurion-web investigation
  - core -> html

------------

## 03/Jul F
- TTN-4335 Update vacancy application page
  - Create sub-task
  - implementing authorization code is the job in TTN-4337
  - Pull request

## 02/Jul T
- Handover aurion-web from Carl & Alex
- TTN-4335 Update vacancy application page
  - Dev
  
## 01/Jul W Annual leave

## 30/Jun T Annual leave

## 29/Jun M Annual leave

------------

## 26/Jun F
- BAMBOO with Ash & CNC

## 25/Jun T
?

## 24/Jun W
- DRM-778 jest test failures on windows os
  - setup test environment (saml server)
  - create the pull request
  - write and share the document: how to run SAML server on PHP built-in web-server

## 23/Jun T
- SEEK Roadmap: Prioritize
- DRM-778 jest test failures on windows os
  - setup test environment (saml server)

## 22/Jun M
- DRM-778 jest test failures on windows os
  code fix

------------
## 19/Jun F
- DRM-770-upgrade-node-to-latest-lts-14.4.0
  fixed, tested, commited and pushed(Paring with Carl)

## 18/Jun T
- SEEK Roadmap
- DRM-770-upgrade-node-to-latest-lts-14.4.0
  - ing... import/extensions
  
  ### rules
  react/jsx-pascal-case
  https://github.com/yannickcr/eslint-plugin-react/blob/master/CHANGELOG.md#7200---2020-05-12
  @typescript-eslint/no-empty-function
  
  Unused eslint-disable directive (no problems were reported from 'import/prefer-default-export')
  C:\ws.aurion.11\aurion-web\packages\api\src\types\index.ts
  C:\ws.aurion.11\aurion-web\packages\mobile\src\screens\leave\types.ts
  
  ## tsc -b
  (Number(queryParams.requested_page)
  .map((child) => child as ReactElement);
  
  
## 17/Jun W
- DRM-770-upgrade-node-to-latest-lts-14.4.0
  - fix: no-multiple-empty-lines & import/no-useless-path-segments
- SEEK Roadmap

## 16/Jun T
- Pair with Carl

## 15/Jun M
- Handover from Dane about Aurion Web
- Handover from Dave about how we work

------------
## 12/Jun F

## 11/Jun T
- write the documents to confluence
  
## 10/Jun W
- Setting Aurion11 environment

## 09/Jun T
- SaaS design
  - tidy code and upload to bitbucket
  - write the document

## 08/Jun M Annual leave

------------
## 05/Jun F
- authorizer
  - re-write typescript
  - make pipeline for building and deploying

## 04/Jun T
- user & tenant manger
  - uploaded to bitbucket
- authorizer
  - make it work

## 03/Jun W
- update usermanger
  - sign-up, create new tenant & role, invite user
  (missing point: inter-service communication)

## 02/Jun T
- test facebook login
  - result: success, easy to set up
  - process: getting the profile data from facebook and store in aws user pool
- pair programming about custom authorizer
- discuss role/feature
- discuss what are the next hurdles/challenges after identity featured in prototype
  - database bottlenecks: split to micro-services, sharding, Aurora Replica
  - batch-run, notification

## 01/Jun M Annual leave

------------
## 29/May F
- building custom authorizer to give a tenant and role based credential -> support the user having multi-tenant
- refresh token with new tenant and role -> so can use identity-pool
(Dane resigns 4 weeks later)

## 28/May T
- thought about how to support user who has multi tenant.
- discussed whether it's worthy or not and how to build.

## 27/May W
- build tenant manager
  - investigate SasS architecture for multi tenant for single user
	: create Identity Pools for every tenant
  
## 26/May T
- build user manager
  - sign-up / sign-in
- think about sso and database isolation
  - handle with two tokens(global and tenant)

## 25/May M
- build user manager
  - design api functions
  - build structure


------------
## 22/May F
- docker build: simple typescript node server
  - git clone https://bitbucket.aurion.io/scm/dp/drp-proto-app-user-manager.git -b dev
- deploy saas back-end infrastructure
  - git clone https://bitbucket.aurion.io/scm/dp/drp-proto-cdk.git -b feature/saas-factory

## 21/May T
- built back-end infra supporing saas using cdk
- to test infra, a simple typescript node server
  - built
  - docker build(~ing)
- had a chat with Dane about the user who has multiple tenants

## 20/May W
- investigate saas factory example
  - work flow among micro-services
  - role/policy based authorization from cognito identity (GetCredentialsForIdentity)
- apigateway lambda authorizer vs api function pipeline authorizer

## 19/May T
- investigate saas factory example

## 18/May M
- read saas factory
	https://github.com/aws-samples/aws-saas-factory-bootcamp
	https://aws.amazon.com/blogs/apn/saas-quick-start-highlights-identity-and-isolation-with-amazon-cognito/
	https://aws.amazon.com/blogs/apn/building-serverless-saas-applications-on-aws/
	https://aws.amazon.com/blogs/apn/multi-tenant-storage-with-amazon-dynamodb/
	https://aws.amazon.com/blogs/apn/modeling-saas-tenant-profiles-on-aws/
	https://aws.amazon.com/blogs/apn/optimizing-saas-tenant-workflows-and-costs/
	https://aws.amazon.com/blogs/apn/migrating-applications-to-saas-a-minimally-invasive-approach/
	https://aws.amazon.com/blogs/apn/migrating-applications-to-saas-rethinking-your-design/

------------
## 15/May F
- watch the video for saas factory: https://www.youtube.com/watch?v=kmVUbngCyOw
  - resources
	- https://aws.amazon.com/quickstart/saas/identity-with-cognito/
	- https://github.com/aws-quickstart/saas-identity-cognito
	- https://aws.amazon.com/partners/saas-on-aws/
	
- read saas factory
- common retro

## 14/May T
- setup new laptop
- reading saas factory: https://github.com/aws-samples/aws-saas-factory-bootcamp
- dreampay standup
  ```
  - create/build/deploy back-end infrastructure with CDK
    - use/set cognito configuration for sign-up/sign-in and authorization
    - use fargate/docker for auto-scaling
    - build java/spring application for company wizard page
  - todo: saas factory, typescript application for comparing to java application
  ```
- Create the document for back-end infrastructure
  - https://confluence.aurion.io/display/PROD/CDK%3A+Back-end+Infrastructure

## 13/May W
- finished java/spring
  - update user service (direct to cognito -> copied dynamodb)
  - environment setting in ecs with cdk
- setup new laptop

## 12/May T
- Migrate user data cognito to dynamodb when signup confirm
- add some data(i.e. default environment) in login token
- pair programming
- finishing java/spring
  - parse login token and pass to request

## 11/May M
- Java in fargate
  - upload normal spring boot application as a docker image to fargate through ecs/ecr
  - try to handover variable to spring application
    - temporarily use application properties in Spring

------------
## 08/May F
- CDK for back-end infra-structure - done
  - apigateway: swagger configuration
- Java/Spring in fargate

## 07/May T
- CDK for back-end infra-structure

## 06/May W
- CDK for back-end infra-structure
  - Auth with Cognito, migrate login infor

## 05/May T
- AWS-ADFS fixed (by Dane)
- Pair Programing
  - Login token issue
- CDK for back-end infra-structure

## 04/May M (Holiday)

------------
## 01/May F
- Try to use AWS-ADFS but failed
- Learning CDK: https://github.com/aws-samples/aws-modern-application-workshop/tree/python-cdk

## 30/APR T
- Clean the resources I've made for the modern web workshop.
- Implementing company wizard page looking similar to KeyPay with schema Dane made. ATM validating input.
- Learning multi-tenant application. benefit: normally bottleneck is on the database.

## 30/APR W
- Modern web workshop
  - ref: https://github.com/aws-samples/aws-modern-application-workshop/
  - Understanding the configuration so deleting
  - VPC: 2 public subnet 2 private subnet => 1 public (1 private)
    - Tolerance test?
- Company wizard
  - 3 or 4 tabs similar to Keypay


------------
...
------------

## 26/03 T
- AWS Amplify

## 25/03 W
- ER Model (Environment, Employee, Pay Group, T900, T901, Allowance, Leave and so like)

## 24/03 T
- elearning
  - Payroll Essentials (120 Mins)
- Dream Pay Introduction and ER Model Overview
  - How STP works. The format for ATO is SBR.
  - ABA: batch transactions format for Bank

## 23/03 M
- elearning
  - Organisation & Position in Core
  - People & Employment (+ hire/terminate) in Core
  - Placement (+ pay scale, banded salary) in Core