# README

## Backend / API Ruby on Rails

### System Description

*Bikes Anonymous* is a small organization that certifies cyclists for riding on the road. They are internationally recognized with clients throughout the world who speak multiple languages. They have certified millions of riders. They run their infrastructure on Azure but use Linux on the back end. The back end consists of an API and an integrated Admin panel. The front end is web-based and interacts with the API.

*BA* has a nightly certification workflow that consists of

1. Receiving a CSV from a partner certification center
2. Converting each row of the CSV into a rider’s licenses in PDF format
3. Emailing the PDF to the license holder using the email field in the CSV
4. Finally, when the whole file has been processed, the system notifies by email both the partner certification center and BA that all certifications in the CSV have been processed. 
Given the amount of data processed on a daily basis, it is imperative that processing the CSV be done via a scheduled task and not as part of the upload process.

Given the relative sensitivity of the data, only authenticated users can upload a file for processing (for this sample project, please only add authentication if you have time, this is low priority for this sample project).

Using **RoR**, create an API and necessary code that fulfils the following user stories.

#### User Stories
* I, as an authenticated user, can upload a CSV so that BA can process the data and mail the cyclist licenses. (Note: for this story, it is not necessary to create a front end, only an endpoint and associated backend code)
* I, as a certified cyclist, can print a PDF of my license so that I can start riding immediately.
* I, as the owner of BA, can read an email containing a summary of the nightly activity so that I can gauge how well my business is doing.

#### Acceptance Criteria
For this exercise, we ask that the developer elaborate the acceptance criteria they deem necessary to verify that the user stories above have been fulfilled.
