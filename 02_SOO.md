# DRAFT
# REQUEST FOR QUOTE #18-0018
# United States Tax Court
# Electronic Filing — Case Management System (EF-CMS)

## Statement of Objectives

### Introduction

The United States Tax Court (hereinafter "Tax Court" or "Court") is an independent Federal court headquartered in Washington, D.C. The Court provides a national forum for the formal adjudication of disputes between taxpayers and the Internal Revenue Service ("IRS"). The vast majority of Federal tax litigation occurs in the Tax Court. Approximately 27,000 cases were initiated in the Tax Court during 2017, and at the end of the year, there were about 22,000 cases pending before the Court. The Court’s mission is to adjudicate the cases pending before it fairly, efficiently, and quickly. [Appendix A further describes the Court’s structure and operations](04_Appendix_A.md).

The Court maintains a data network that operates in a Windows environment and supports approximately 250 internal users. [Appendix B describes the Court’s current network environment](05_Appendix_B.md) in more detail.

The Court currently uses a legacy case management system that is not web-based. The Court holds a license to use the software that supports that system. Under the terms of that license, the Court is precluded from disclosing any programs, concepts, designs, or source code. This may be an important operating constraint for the Contractor because it will not be able to view or access the current system in any way.

The Court intends to deploy a new web-based electronic filing and case management system (hereinafter "EF-CMS" or "System") and transition from its current case management system at the earliest opportunity. The Court requests quotes from GSA Schedule 70 vendors to provide agile development services to develop that System.

Award will be made to the single Offeror whose proposal represents the best value to the Court. The Court intends to issue a Time-and-Materials type purchase order under an existing General Services Administration (GSA) Schedule Information Technology 70 (IT 70) contract, under SIN 132-51. The order will be for an initial period of one (1) year, and the Court will have options to extend the initial period for a total of up to two (2) additional years.

The Court will pay a not to exceed amount of up to $2 million for services and authorized travel during the first year, and up to $2 million for services and authorized travel during each of the two option years.

**Quotes are due by [TBD] and must be submitted electronically to clerk@ustaxcourt.gov.**

### Description of Work to be Performed

The Contractor must provide services that will include all aspects of the software development process, including initial planning, design, software development and coding, prototyping, documentation, testing, configuration, and deployment into the Court’s pre-production environment. The Contractor must use free, open-source software whenever possible. The Court intends that the code developed as a result of this project will be committed to the public domain.

This software development project will follow agile development principles, using free and open-source software, robust documentation, human-centered design, and an extensible infrastructure. The Court expects that the development process will be collaborative and iterative, with open, regular, and frequent communication between the Court and the Contractor. The Court has designated an employee who will be empowered to serve as the Product Owner for this project. The Court could also provide an individual with prior experience to serve as the Scrum Master for this project. Additional Court representatives will also be promptly available as needed to assist in the development process, including for user testing.

The Court expects the development process will consist of 2-week sprint cycles, and that the initial phases of the development process will focus on providing identity and access management, case initiation, payment of fees, search functionality, e-signatures, notes, and content management.

The Court intends to deploy the new System and convert operations from the current system as soon as the software for the new System has been sufficiently developed to provide the minimal functionality required to support the Court’s basic operations. The Court expects that development of the software and modification to the System will continue after this deployment and conversion.

### General Requirements

System Requirements — The Court’s future EF-CMS will be cloud-based and will have an intuitive web-based interface that is accessible from both internal and external platforms, including desktops, laptops, tablets, and mobile devices. The System will have no single point of failure. The System will use elastic, dynamically-allocated computing resources that respond to changing demand. The System will include user authentication and authorization functionality that uses open source encryption protocols.

Software Requirements — The software architecture must be extensible to allow for future development. The code base must incorporate analytics, monitoring, continuous integration, and measurement tools. The Contractor must use plain language in application design and development whenever possible. The Contractor will not be responsible for hosting of the system or obtaining an Authority to Operate (ATO). The Contractor must post all developed code to a GitHub repository designated by the Court.

### Deliverables and Performance Standards

The code and documentation to be provided by the Contractor must meet the performance standards and quality levels listed below. The Court will assess the standard and quality levels of the code and documentation using the methods set forth below.

| Deliverable | Performance Standard(s) | Acceptable Quality Level | Method of Assessment |
| --- | --- | --- | --- |
| Tested Code | Code delivered under the order must have substantial test code coverage and a clean code base Version-controlled Court GitHub repository of code that comprises product that will remain in the government domain | Minimum of 90% test coverage of all relevant code | Combination of manual review and automated testing |
| Properly Styled Code | [GSA 18F Front End Guide](https://frontend.18f.gov/#js-style) | 0 linting errors and 0 warnings | Combination of manual review and automated testing |
| Accessible | Web Content Accessibility Guidelines 2.0 AA (WCAG 2.0 AA) standards | 0 errors reported for WCAG 2.0 AA standards using an automated scanner and 0 errors reported in manual testing | [http://squizlabs.github.io/HTML\_CodeSniffer/](http://squizlabs.github.io/HTML_CodeSniffer/) or [https://github.com/pa11y/pa11y](https://github.com/pa11y/pa11y) |
| Deployed | Code must successfully build and deploy into staging environment. | Successful build with a single command | Combination of manual review and automated testing |
| Documentation | All dependencies are listed and the licenses are documented. Major functionality in the software/source code is documented. Individual methods are documented inline using comments that permit the use tools such as JsDoc. System diagram is provided. | Combination of manual review and automated testing, if available | Manual review |
| Secure | OWASP Application Security Verification Standard 3.0 | Code submitted must be free of medium- and high-level static and dynamic security vulnerabilities | Clean tests from a static testing SaaS (such as Gemnasium) and from OWASP ZAP, along with documentation explaining any false positives |

### User Stories

[Appendix C consists of text and diagrams that present the case processing workflows](Appendix_C.md) that the Court currently expects to eventually be supported by a future EF-CMS. The Court expects that these expected case processing workflows will change during the development process.

The set of preliminary user stories set forth below will be the starting point for the software development services to be provided under this order. These user stories are provided only for illustrative purposes, and do not comprise the scope or detail of the work that will be performed. Additional user stories to be determined will likely cover areas including e-signatures, notes, routing, notifications, calendaring, and reporting and analytics.

The backlog of user stories will be maintained in a web-based project management application that will be provided by the Court. Individual user stories may be modified, added, retracted, or reprioritized by the Court at any time, and the Court expects that the user stories will be continuously refined during the development process. This set of preliminary user stories has been categorized into releases, but has not been prioritized.

### Case Initiation

- As a Pro Se Petitioner, I need to initiate a case by filing an electronic petition so I can seek resolution of my dispute with the IRS.
- As a Pro Se Petitioner, I need to initiate a case by filing a paper petition so I can seek resolution of my dispute with the IRS.
- As a Member of the Tax Court Bar, I need to initiate a case on behalf of my client by filing an electronic petition so my client can seek resolution of their dispute with the IRS.
- As a Member of the Tax Court Bar, I need to initiate a case on behalf of my client by filing a paper petition so my client can seek resolution of their dispute with the IRS.
- As an Executor of an Estate, I need to initiate a case by filing an electronic petition so I can seek resolution of the estate’s tax issue.
- As an Executor of an Estate, I need to initiate a case by filing a paper petition so I can seek resolution of the estate’s tax issue.
- As the Tax Matters Partner of a partnership, I need to initiate a case by filing an electronic petition so I can seek resolution of the partnership’s tax issue.
- As the Tax Matters Partner of a partnership, I need to initiate a case by filing a paper petition so I can seek resolution of the partnership’s tax issue.
- As an electronic filer, I need to submit my documents under seal so I don’t inadvertently disclose sensitive or confidential information.
- As Clerk of the Court, I need to have a party code associated with each party so I can track them in the System.
- As a Petitioner, I need to select a place of trial so my case can be tried at a convenient location.

### Fees

- As a Pro Se Petitioner, I need to pay my filing fee so my case can proceed, or submit a request for fee waiver.
- As a Member of the Tax Court Bar, I need to pay the filing fee on behalf of a client so their case can proceed, or submit a request for fee waiver on behalf of a client.
- As a Member of the Tax Court Bar, I need to pay my bar fees to maintain an active status.
- As disinterested person, I need to request and pay for copies of existing case filings of record and court publications/related documents so I can better familiarize myself with court actions for purposes of legal research, and familiarize myself with the rules of practice and procedure.
- As an individual seeking admission to the Tax Court Bar, I need to pay an application fee and/or a non-attorney exam fee so I can become admitted to the Court’s bar.
- As Staff, I need to determine whether payment has been made so I can take the proper action on a case/application.

### View & Search

- As an Internal Court User, I need to view case records and all filings in all unsealed cases so I can take proper action on a case.
- As an Internal Court User with authorized access, I need to view case records and all filings in sealed cases so I can take proper action on a case.
- As a Pro Se Petitioner, I need to view docket records and all filings in my case so I can appropriately prosecute my case.
- As a Member of the Tax Court Bar, I need to view dockets record and all filings in cases in which I am counsel of record so I can appropriately prosecute my client’s case.
- As a Member of the Public, I need to search case records so I can keep abreast of Tax Court cases.
- As Clerk of the Court, I need to ensure that only authorized Internal Court Users can view case records and filings in sealed cases.
- As Clerk of the Court, I need to ensure that only permissible search results are available to the public so I don’t accidentally provide inappropriate information to unauthorized users.

### Content Management

- As Staff, I need to be able to scan and upload paper documents so I can store and process them electronically.
- As a Pro Se Petitioner, I need to electronically file documents so I can seek resolution of my dispute with the IRS.
- As a Pro Se Petitioner, I need to file paper documents so I can seek resolution of my dispute with the IRS.
- As a Member of the Tax Court Bar, I need to electronically file documents so I can seek resolution of the client’s dispute with the IRS.
- As a non-party in a case, I need to electronically file various documents, such as amicus briefs, motions to quash subpoenas, notices of elections to participate in a partnership case, or motions to intervene, so I can participate in an existing tax court case.
- As a court user, I need template orders and notices so I can streamline my work.
- As a court user, I need the ability to create free form orders and notices so I can properly address issues in a case.
- As Clerk of the Court, I need to have event codes associated with each type of court filing so I can track them in the System.
- As an electronic filer, I need to attach documents for filing in my case so they can become part of the record.
- As a court user, I need to attach documents to orders and notices so they can become part of the record.
- As a court user, I need to see all user activity related to a case so I can monitor workflows.

## Location of Work to be Performed

The Contractor may choose the location(s) from which to perform the required software development services. All Tax Court judges and staff are based in Washington, D.C. The Court’s hours of operation are 8:00 a.m. to 4:30 p.m. Eastern Time. The Court’s Product Owner and other Court representatives will be available to confer with Contractor representatives by video connection on a daily basis during the development process. In addition, the Court is willing to make space available on a daily basis for up to seven (7) Contractor representatives at the Court’s main building in D.C.

## Order Type and Ceiling Price

This is a time and materials order and all quotes must be submitted on this basis. The Court will pay a not to exceed amount of up to $2 million for services and authorized travel during the first year, and up to $2 million for services and authorized travel during each of the two option years.

## Period of Performance

Performance shall be for an initial period that begins with the date of order and ends one (1) year after the date of order. The Court may, by written notice issued at least 15 days prior to expiration of the initial period, extend the period of performance for an additional year. If the Court exercises that initial option, the Court may also, by written notice issued at least 15 days prior to the expiration of the initial option year, extend the period of performance for an additional year.

## Delivery Instructions

The Contractor must deliver software code at least daily to the Court’s GitHub repository. Document deliverables must be submitted to the Court electronically at [clerk@ustaxcourt.gov](mailto:clerk@ustaxcourt.gov).

## Special Requirements

Travel — The Tax Court will reimburse expenses relating to travel necessary to provide the professional services required under the order, up to a ceiling of $50,000 per year, so long as each expense is approved in advance by the Court. To be eligible for reimbursement, those travel expenses must be allowable under the Federal Travel Regulations promulgated by the General Services Administration in effect at the time the travel was taken.

Key Personnel — The Contractor must designate both a Project Manager (PM) and a Technical Lead as Key Personnel for this project. The PM will be a direct liaison to the Court product team, and will be responsible for the supervision and management of all of the Contractor’s personnel, technical assistance, and interface. The Technical Lead must have a full understanding of the technical approach to be used by the development team and will be responsible for ensuring that the development team follows that approach.

Key Personnel Substitution — Key Personnel substitutions must be approved by the Court in writing, and will only be justified by a Court request, sudden illness, death, change of employment, or termination of employment for cause. Any Contractor request for substitutions of Key Personnel must include a detailed explanation of the circumstances necessitating the proposed substitution, and a complete résumé for the proposed substitute or addition, including skills, experience, education, training, and security level. The Court’s failure to approve the proposed substitution will not constitute grounds for non-performance by the Contractor, or form a valid basis for any claim for money or any equitable adjustment.

Teaming Arrangements — Teaming arrangements are permitted. The successful Offeror will be the prime contractor under this order, regardless of any teaming arrangements. The successful Offeror will be solely responsible for providing the required services, and payments will be made only to the successful Offeror.

Data Rights and Ownership of Deliverables — The Court intends that any software or documentation created as a result of the services provided under this order be committed to the public domain. That includes, but is not limited to, data, documents, graphics, code, plans, reports, schedules, schemas, metadata, architecture designs, and the like; all new open source software created by the Contractor and forks or branches of current open source software where the Contractor has made a modification; and all new tooling, scripting configuration management, infrastructure as code, or any other final changes or edits to successfully deploy or operate the software.

The Contractor must use free, open source technologies wherever possible, consistent with the [GSA 18F Source Code Policy](https://18f.gsa.gov/open-source-policy/), with licenses that meet [the Open Source Initiative’s "Open Source Definition](https://opensource.org/osd)." Any use of licensed software in the development process must be promptly disclosed to the Court in writing, and must be clearly listed in the documentation.

If the Contractor seeks to use software that does not have an open source license, the Contractor must obtain permission from the Court, in writing, before using that software in any way in the development process. If the use of non-open source software is approved, all license rights must be promptly assigned to the Court.

If an open source license used in the development process provides implementation guidance, the Contractor must ensure compliance with that guidance. If implementation guidance is not provided, the Contractor must attach or include the license within the work itself, such as in code comments at the beginning of a file, or code comments contained in a license file within a software repository.

Contractor Access — The Tax Court shall have and exercise full and complete control over granting, denying, withholding, and terminating access of Contractor representatives to Tax Court facilities and Tax Court IT resources. The Court may prohibit access to Tax Court facilities or IT resources by a Contractor representative if the Court deems access by that Contractor representative to be contrary to the public interest for any reason, including, but not limited to, carelessness, insubordination, incompetence, or security concerns. All Contractor representatives working on-site at Court facilities will be required to have completed and passed a limited criminal background suitability check, and may be subjected to additional FBI screening and U.S. Marshal inspection.

Invoices — Invoices for services and/or travel expenses must be submitted to the address (physical or e-mail) specified by the Court. To constitute a proper invoice, the billing document must include the following information and/or attached documentation:

(1) Name of Contractor and Contractor’s Taxpayer Identification Number;

(2) Period covered by invoice and invoice date;

(3) Purchase order number;

(4) All invoices for services must set forth in detail the following:

&nbsp;&nbsp;&nbsp;(i) Individual performing service each day by hour and quarter of an hour;

&nbsp;&nbsp;&nbsp;(ii) Type of services performed each day by hour and quarter of an hour; and

&nbsp;&nbsp;&nbsp;(iii) Hourly rate for each service so detailed;

(5) Any applicable payment discount terms; and

(6) Total amount billed.

All follow-up invoices must be marked "Duplicate of Original."

Public Use of the Name of the Tax Court — The Contractor may not publicly release information pertaining to this order without prior written approval from the Contracting Officer. The Contractor shall not refer to the Tax Court in advertising, news releases, brochures, catalogs, letters of reference, web sites, or any other media, in such a way as to represent or imply that the Court prefers or endorses the services offered by the Contractor. However, the Contractor may refer to the Court as one of its customers when providing past performance information as part of a quote or proposal submission.
