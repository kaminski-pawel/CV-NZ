# Pawel Kaminski

## Objective

Looking for a full-time work as Software/Application Programmer in New Zealand (on-location).

## Education

Master's Degree (LLM) at UAM Law School in Poznan, Poland (the third best Law School in the country).

## Work history

I have been using Python, SQL and VBA at work since 2016, JavaScript since 2019. Since 2018 around 90% of my workhours involves writing software.

- 2018-2022 - self-employed
- 2014-2018 - Tax Consultant at TPA Poland (Baker Tilly Group)
- 2011-2014 - Lawyer at Merski Radcy Prawni i Adwokaci Sp.k. Law Firm

## Project history

### 2022 - Twitterbot based on AWS SQS

Twitter Bot, which publishes posts of companies' business activities.

This bot utilizes a FIFO queue. First, a tweet is prepared and queued to AWS Simple Queue Service. Then, after a certain amount of time, the tweet is dequeued and published using Twitter API.

- Python
- boto3, tweepy
- AWS SQS

### 2022 - AWS Lambda functions for serving as an backend API

This project consists of two AWS Lambda functions to provide an API to the list of companies maintained by Jeffrey Sonnenfeld and his team the Yale Chief Executive Leadership Institute.

- Python
- JavaScript
- Docker
- AWS Lambda, DynamoDB, ECR

### 2022 - horizontal waterfall chart

Horizontal waterfall chart for use in a larger project.

- JavaScript
- chart.js

### 2022 - prototypes of using IndexedDB and Web Workers

Prototypes include: the combination of React with IndexedDB, MobX and StateX, as well as using Web Workers in Nuxt.

### 2021 - 2022 - Timesheet & Project Management Software

Timesheet and project management software tailored to the needs of financial auditors.

Technically, it is a Python and Django application based on a PostgreSQL database. Interesting in this project is the use of React mini applications as reactive widgets. Instead of writing a full-fledged front-end application the React apps are bundled with Webpack to 'vanilla' JavaScript files, which Django serves inside of a HTML script tag.

- Python
- Django
- JavaScript
- React
- Webpack, Babel
- PostgreSQL
- AWS RDS, EC2

### 2021 - mass mailing software based on AWS SES

For the purpose of a mass mailing marketing campaign, I wrote an application that takes in as an input an HTML email template file and sends multiple emails customized to different recipients. This project uses Amazon Simple Email Service (SES).

- Python
- AWS SES
- libraries: boto3, bs4, email, jinja2
- mail security (SPF, DKIM)

### 2021 - Website with profiles of road construction companies

In cooperation with the Polish Chamber of Commerce for Road Engineering I wrote a website presenting financial profiles of road construction companies.

The front-end is a JavaScript/Nuxt application rendered on a server side. The financial data of the companies is loaded from the Amazon DynamoDB database (project was maintained only for several months, some links might not work, especially links to resources in S3 buckets).

- Python
- Django
- JavaScript
- Vue, Nuxt
- AWS DynamoDB, S3

### 2021 - Operating margin prediction software

The aim of this project was to help software house companies to find the most profitable combination of specializations.

To do this, I exported financial results of software house companies using mojeanalizy.pl and extracted data from clutch.co website to find out which technologies these companies use and which markets they address. Next, I wrote a linear regression model that predicts the expected operating margin, taking into account the variables entered by the user (e.g. service lines, industry focus). This solution was supposed to allow users to tweak company's specialization to find the highest operating margin. I made a proof of concept for the client, but the full version was never commissioned due to budget concerns.

- Python
- Django
- Selenium
- pandas, sklearn

### 2021 - Scraping using AWS Lambda

A fork of an AWS Lambda function with Chromium webdriver modified to scrape Bisnode economic information office website in order to extract public data requested by a client.

- Python
- Docker
- Selenium
- AWS Lambda

### 2021 - Scraping despite ReCaptcha

A software scraping public records from the state aid registry. An interesting part of this project is the use of a ReCaptcha solver.

- Python
- Selenium

### Public procurement analysis

// TODO

### 2020 - 2022 - Advanced scraping software

In Poland, financial statements of companies and other institutions are de jure publicly available, but de facto difficult to access and analyse.

I created an application that downloads financial reports while avoiding denial of access to these public resources. Most difficulties of the project stem from the need to prevent blacklisting while ensuring that the process is legal and ethical. On the technical side, this is achieved by making the automatic scraper to behave like a normal user. This includes sending spaced HTTP requests with appropriate HTTP headers, randomizing behaviour, accessing the registry from different IP addresses. From an architectural perspective, the software follows the Page Object Model pattern.

- Python
- Selenium
- proxy servers
- Docker
- AWS EC2, ECR

### 2020 - Simple scraping tool

A simple tool for extracting contents of the public registry Court and Commercial Gazette.

- Python
- Selenium

### 2019 - 2022 - mojeanalizy.pl

Tools for reading and analyzing financial statements of Polish companies and other institutions, which are stored in XML files defined according to various XSD schemes.

By far the most complex software I've ever written. The backend consists of small modules grouped into entities layer and application layer. Among others, it consists of the following features:

- reading XML files with financial statements
- exporting contents of XML files to .XLSX (Excel) or .CSV files
- ratio analysis (indebtness, profitability, margins, liquidity, cash conversion cycle, transfer pricing, etc.)
- bankruptcy prediction
- standardization of financial data
- verification of financial statements
- fixing minor errors of financial statements
- company's use of a tax shield

Financial data read by the software can be visualised (incl. as a chart), printed and saved as an Excel file. The tools allow to analyse financial data from one or many financial statements. With thousands unique users a month the application is widely used across the country among managers, journalists and finance professionals (accountants, auditors, analysts, etc.).

- Python
- Django, Django Rest Framework
- bs4, xlsx, unittest
- JavaScript, TypeScript
- Web Services, Web Workers, PWA
- Vue, Nuxt
- D3, chart.js
- cypress, jest

### 2019 - API client

Client for making requests to the Central Statistical Office API and copying its databases.

- Python

### 2018 - 2022 - Pandas analysis services

Transfer pricing documentation required from Polish taxpayers includes a 'Comparability Analysis'.

I provide services for performing appropriate calculations using Python and pandas. Examples of such calculations include: a) establishing at what median unit price a company sells its products to affiliated and non-affiliated companies, b) determining the profitability ratios of the controlled subsidiaries and comparing them with uncontrolled companies.

- Python
- pandas

### 2018 - OCR and NLP analysis

In 2018, I wrote small tools for optical character recognition and natural language processing, especially table detection and text mining, as well as keyword extraction.

- Python
- Tesseract

### 2018 - MS Access application for calculating amortization schedule under IFRS 16

International Financial Reporting Standards 16 (IFRS 16) introduced a new approach to accounting for leases. Companies that kept their books of account as per IFRS standards had to change their amortization schedules.

The software I wrote calculated the correct amortization schedules and amounts to include in the financial statement. It also generated accounting documents. The software comprised of a) central back-end .ACCDB application consisting of relational database, b) front-end .ACCDB application serving as a GUI (forms, reports, etc.) to be copied onto users local computers, c) a VBA script to update local front-end applications with changes made to the central database. Both back-end and front-end applications were password protected and supported different levels of authorization.

- VBA
- SQL

### 2017 - 2018 - expert system for generating .DOCX reports

Polish law requires taxpayers to prepare robust transfer pricing documentation, i.e. a detailed specification of all major transactions between subsidiaries, affiliates or commonly controlled companies that are part of the same larger enterprise.

In 2018-2019, I wrote an expert system in which a user went through a dynamically rendered form wizard, answered questions about a transaction to be documented, and the program generated a .DOCX document compliant with the requirements of the law.

- Python
- Django

### 2017 - Django based API client

In 2017, a new requirement for Polish VAT taxpayers was introduced. Under the new regulations, in order to comply the taxpayers had to check each trading partner if he/she was on the blacklist provided by the government. To help taxpayers who had hundreds and thousands of trade partners, I build a simple service that allowed to check them all at once.

Under the hood, this service took .XLSX file as an input, iterated over the contents of the file and sent a request to the WSDL service provided by EU European Commission. The result was a report in PDF format. The service was used only locally and for a short time before it was replaced by a commercial product.

- Python
- Django
- libraries: openpyxl, xhtml2pdf, etc.

### 2016-2018 - scripts for populating MS Word .DOCX files

As a lawyer I had to draft many legal documents from predefined templates. I automated this process by writing several Python CLI scripts, which opened .DOCX template files and replaced the placeholder values with the corresponding data.

The scripts took advantage of the fact that .DOCX files are just zip archives that contain strictly defined XML files. The scripts were accessible from the command line and did not have a GUI.

- Python

### 2014 - 2017 - small VBA scripts and Macros

When I worked as a tax consultant, I worked on .XLSX (MS Office Excel) and .ACCDB (MS Office Access) files, sometimes using VBA and macros. Examples of such use are: tax and accounting calculations, occasionally fetching some external data like appropriate exchange rates into Excel spreadsheet. Rarely I had to write raw SQL queries for handling a database in MS Access.

- VBA
- SQL

## Visa status

Looking for a job offer from an employer who is accredited to hire migrants for the Accredited Employer Work Visa.

## Other skills

- English ⭐⭐⭐
- Polish ⭐⭐⭐
- German ⭐⭐
- Russian ⭐
- Scrum, Agile
- Git, Github, Jira, Bitbucket
