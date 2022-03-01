---
Start Date: 26th Feb 2022
Trello Link: 
tags: feature
---

## Description (High Level)

This database will act as store of job data. 

---

## Goals

^e7aac0
The goal of this database is to act as a store of job market data. 

This should be:

- Free
- Queried via serverless functions

---

## Tasks / Features List

^624345
### Essential
These are the tasks and features that are required for the main functionality of project to be achieved.

#### Determine Data Fields
The data fields that I plan to capture/read are: ^a60a69
- Gross Salary
	- Monthly/Yearly
- Industry: [Careers | List of Careers and Occupations to Explore [Updated for 2021-2022] (recruiter.com)](https://www.recruiter.com/careers/)
- Job Title:
Code to pull job industry and title information from [Careers | List of Careers and Occupations to Explore [Updated for 2021-2022] (recruiter.com)](https://www.recruiter.com/careers/)

```js
var jobTitles = document.querySelectorAll(".title-h3-career")
var jobTitlesList = []
jobTitles.forEach(e => {
    jobTitlesList.push(e.textContent)
    
})
jobTitlesList;

```
- \# of Years in position
- Degree Category
- Job Level
	- Entry-level
	- Supervisor
	- Middle-Management
	- Senior Management  
- Hours Worked
- Job Satisfaction
- [[Read Data]]
- [[Add Data]]

### Non-Essential
These are the tasks and features that are not required for the main functionality of project to be achieved but add additional functionalities to the project. 
- [[Prevent Data Duplication]]
- [[]]
---
## Technologies to Use
I plan to use SteinHQ to act as the database API which uses Google Sheets as the data store. 

---


## Timeline

---
## Resources
- [Turn Google Sheets into a database API. Ship fast and manage your data with ease - Stein (steinhq.com)](https://steinhq.com/)
- [sheet.best · Turn your google sheets into a REST API](https://sheet.best/)
- [Google Sheets REST API, connect Google Spreadsheet with your site (sheetdb.io)](https://sheetdb.io/)

