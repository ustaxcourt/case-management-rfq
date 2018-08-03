# REQUEST FOR QUOTE #18-0018
# United States Tax Court
# Electronic Filing — Case Management System (EF-CMS)

## Statement of Work

### Introduction

The United States Tax Court (hereinafter “the Tax Court” or “the Court”) is an independent Federal court in Washington, D.C, that provides a national forum for the formal adjudication of disputes between taxpayers and the Internal Revenue Service (“IRS”). The Court’s mission is to adjudicate the cases pending before it fairly, efficiently, and quickly. The Court’s operations and organization are described in Appendix A.

The Court currently uses a legacy case management system that is non-web-based and operates through desktop applications installed on individual workstations. The Court intends to develop and deploy a new web-based electronic filing and case management system (hereinafter “EF-CMS” or “the System”). The case processing workflows that the Court expects the System to support are described in Appendix B.

The Court is requesting quotes for agile software development services from vendors with contracts under GSA Schedule 70, SIN 132-51. The Court is sending this Request for Quote (RFQ) by email to certain vendors with contracts under GSA Schedule 70, SIN 132-51, who may have particular expertise in software development projects. The Court is also posting this RFQ on the Court’s GitHub site ([*https://github.com/ustaxcourt/case-management-rfq*](https://github.com/ustaxcourt/case-management-rfq)). The Court will consider quotes from any vendor that has a contract under GSA Schedule 70, SIN 132-51. The Court may award a task order under an existing GSA Schedule 70 contract to the single Offeror whose proposal represents the best value to the Court.

The Court is prepared to pay up to \$2 million for services and authorized travel incurred under the task order during the initial one-year performance period, and up to an additional \$2 million for services and authorized travel incurred during each of two Court option years.

The Court has worked closely with representatives of 18F (GSA) and the MITRE Corporation in preparing this RFQ.

**Quotes are due by 5:00 p.m. EDT, Friday, August 24, 2018, and must be submitted by email to [clerk@ustaxcourt.gov](mailto:clerk@ustaxcourt.gov).**

### Description of Work to be Performed

The Court seeks agile software development services. The services to be provided will include all aspects of the software development process, including initial planning, design, software development and coding, prototyping, documentation, testing, and configuration.

The Court intends that the software delivered under this task order will be committed to the public domain. The Contractor will have to obtain Court permission before delivering software under this task order that incorporates any software that is not free and open source. The Contractor must post all developed code to a GitHub repository designated by the Court. The Contractor will not be responsible for importing any pending case data, practitioner data, or other data into the new System.

This software development project will use agile development principles, with robust documentation, human-centered design, and an extensible infrastructure. The Court expects that the development process will be collaborative and iterative, with open, regular, and frequent communication between the Court and the Contractor. The Court expects that the development process will consist of 2-week sprint cycles, and that the initial phases of the development process will focus on providing identity and access management, case initiation, payment of fees, search functionality, e-signatures, notes, and content management.

The Court has designated an employee who will be empowered to serve as the Product Owner for this project. That individual has been certified by the Scrum Alliance as a Certified Scrum Product Owner (CSPO). The Court’s Product Owner will set direction, make prioritization choices to build a product roadmap, consider and address the business needs of the Court, and support the other members of the development team. The Contractor will assist the Court with product management.

The Court is also willing to provide an individual with prior experience to serve as the Scrum Master for this project. Additional Court representatives will be promptly available as needed to assist in the development process, including for internal user testing. The Court will arrange for any necessary external user testing.

The Court’s current internal management and staffing levels are not adequate to allow for effective coordination with more than one development team, at least during the initial stages of the development process. If the development process goes smoothly and it appears the Court has sufficient capability, the Court may consider adding a second Contractor development team.

The Court, not the Contractor, will be responsible for the hosting of the deployed System and obtaining any necessary Authority to Operate (ATO). The Court will also determine what security controls are required and whether they have been satisfied. The Court expects to provide those security controls to the Contractor as either acceptance criteria or separate user stories. The Contractor is expected to use best practices for security in delivering code.

The Court holds a license to use the software that supports the legacy system. Under the terms of that license, the Court is precluded from disclosing any programs, concepts, designs, or source code. Therefore the Contractor will not be able to view or access the current system (except for those aspects that are currently accessible by the public), and it will not be feasible to deploy the new System using an incremental approach. In addition, the Court does not intend to operate the legacy system and the new System in tandem.

The Court intends to deploy the new System and convert case management operations from the current system as soon as the software for the new System has been sufficiently developed to provide the minimal viable functionality required to support an acceptable level of the Court’s fundamental case management operations. This minimal viable functionality will include the ability for external users to file documents electronically (including case initiation documents), and the ability for internal Court users to route those filings appropriately, take action on those filings, and serve filings and orders on the parties and their representatives. The Court intends for the software to have been sufficiently developed to allow deployment and conversion by September 30, 2019. The Court expects that substantial further development of the software and modifications to the System will occur after this deployment and conversion.

### General Requirements

*System Requirements* – The System will be hosted on a FedRAMP-certified cloud storage solution controlled by the Court. The System must incorporate an intuitive web-based interface that is accessible from both internal and external platforms, including desktops, laptops, tablets, thin/zero clients, and mobile devices. The System architecture must incorporate Application Programming Interfaces (APIs) to intermediate major components. The System must have no single point of failure. The System will use elastic, dynamically-allocated computing resources that accommodate changing demand in real time. The System must include user authentication and authorization functionality that uses open source encryption protocols. The Court does not currently have any enterprise authentication/authorization mechanisms that need to be integrated into the new System, but the Court expects these mechanisms to be developed as part of a future System-level user story. The System must be integrated with pay.gov to enable the receipt of payments.

*Software Requirements* – The software architecture must be extensible to allow for future development. The code base must incorporate analytics, monitoring, continuous integration, and measurement tools. Application design and development must use plain language to the extent practical.

*Environments* – The Court will be responsible for creating, maintaining, and managing an internet-connected staging environment, and an internet-connected production environment, on a FedRAMP-certified cloud storage solution. The Contractor will be responsible for creating, maintaining, and managing its own internet-connected development environment, which will be the only environment that the Contractor will deploy to. The Contractor’s development environment must mirror the Court’s staging and production environments.


### Deliverables and Performance Standards

The following chart sets forth the performance standards and quality levels the code and documentation provided by the Contractor must meet, and the methods the Court will use to assess the standard and quality levels of that code and documentation.

| Deliverable | Performance Standard(s) | Acceptable Quality Level | Method of Assessment |
| --- | --- | --- | --- |
| Tested Code | Code delivered under the order must have substantial test code coverage and a clean code base<br><br>Version-controlled Court GitHub repository of code that comprises product that will remain in the government domain | Minimum of 90% test coverage of all relevant code | Combination of manual review and automated testing |
| Properly Styled Code | [GSA 18F Front End Guide](https://frontend.18f.gov/#js-style) | 0 linting errors and 0 warnings | Combination of manual review and automated testing |
| Accessible | Web Content Accessibility Guidelines 2.1 AA (WCAG 2.1 AA) standards | 0 errors reported for WCAG 2.1 AA standards using an automated scanner and 0 errors reported in manual testing | [http://squizlabs.github.io/HTML\_CodeSniffer/](http://squizlabs.github.io/HTML_CodeSniffer/) or [https://github.com/pa11y/pa11y](https://github.com/pa11y/pa11y) |
| Deployed | Code must successfully build and deploy into staging environment. | Successful build with a single command | Combination of manual review and automated testing |
| Documentation | All dependencies are listed and the licenses are documented. Major functionality in the software/source code is documented. Individual methods are documented inline using comments that permit the use tools such as JsDoc. System diagram is provided. | Combination of manual review and automated testing, if available | Manual review |
| Secure | OWASP Application Security Verification Standard 3.0 | Code submitted must be free of medium- and high-level static and dynamic security vulnerabilities | Clean tests from a static testing SaaS (such as Gemnasium) and from OWASP ZAP, along with documentation explaining any false positives |

### User Stories

The set of preliminary user stories set forth below will be the starting point for the development of software to be provided under this task order. These preliminary user stories are provided only for illustrative purposes, and do not comprise the full scope or detail of the project. They have been grouped by topic, but have not been prioritized.

The Court expects that the Contractor will work closely with the Product Owner to perform user research, prepare user personas, and to develop and prioritize a full gamut of user stories as the project progresses. The Court also expects that the Contractor will work closely with the Product Owner and Court-provided end-users to perform usability testing at regular intervals throughout the development process.

Individual user stories may be modified, added, retracted, or reprioritized by the Court at any time, and the Court expects that the user stories will be continuously refined during the development process. Additional user stories will likely cover areas such as e-signatures, notes, routing, notifications, calendaring, and reporting and analytics.

The backlog of user stories will be maintained in JIRA, a web-based project management application, that will be provided by the Court. The Contractor will be required to manage and update user stories using JIRA.

[Appendix B consists of text and diagrams that present the case processing workflows](05_Appendix_B.md) that the Court currently expects to eventually be supported by a future EF-CMS. The case processing workflows set forth in Appendix B may be revised during the development process.

#### Case Initiation

-   As a Pro Se Petitioner, I need to initiate a case by filing an electronic petition so I can seek resolution of my dispute with the IRS.
-   As a Pro Se Petitioner, I need to initiate a case by filing a paper petition so I can seek resolution of my dispute with the IRS.
-   As a Member of the Tax Court Bar, I need to initiate a case on behalf of my client by filing an electronic petition so my client can seek resolution of their dispute with the IRS.
-   As a Member of the Tax Court Bar, I need to initiate a case on behalf of my client by filing a paper petition so my client can seek resolution of their dispute with the IRS.
-   As an Executor of an Estate, I need to initiate a case by filing an electronic petition so I can seek resolution of the estate’s tax issue.
-   As an Executor of an Estate, I need to initiate a case by filing a paper petition so I can seek resolution of the estate’s tax issue.
-   As the Tax Matters Partner of a partnership, I need to initiate a case by filing an electronic petition so I can seek resolution of the partnership’s tax issue.
-   As the Tax Matters Partner of a partnership, I need to initiate a case by filing a paper petition so I can seek resolution of the partnership’s tax issue.
-   As an electronic filer, I need to submit my documents under seal so I don’t inadvertently disclose sensitive or confidential information.
-   As Clerk of the Court, I need to have a party code associated with each party so I can track them in the System.
-   As a Petitioner, I need to select a place of trial so my case can be tried at a convenient location.

#### Fees

-   As a Pro Se Petitioner, I need to pay my filing fee so my case can proceed, or submit a request for fee waiver.
-   As a Member of the Tax Court Bar, I need to pay the filing fee on behalf of a client so their case can proceed, or submit a request for fee waiver on behalf of a client.
-   As a Member of the Tax Court Bar, I need to pay my bar fees to maintain an active status.
-   As a disinterested person, I need to request and pay for copies of existing case filings of record and court publications/related documents so I can better familiarize myself with court actions for purposes of legal research, and familiarize myself with the rules of practice and procedure.
-   As an individual seeking admission to the Tax Court Bar, I need to pay an application fee and/or a non-attorney exam fee to be admitted to the Court’s bar.
-   As Staff, I need to determine whether payment has been made so I can take the proper action on a case/application.

#### View and Search

-   As an Internal Court User, I need to view case records and all filings in all unsealed cases so I can take proper action on a case.
-   As an Internal Court User with authorized access, I need to view case records and all filings in sealed cases so I can take proper action on a case.
-   As a Pro Se Petitioner, I need to view docket records and all filings in my case so I can appropriately prosecute my case.
-   As a Member of the Tax Court Bar, I need to view docket records and all filings in cases in which I am counsel of record so I can appropriately prosecute my client’s case.
-   As a Member of the Public, I need to search case records so I can keep abreast of Tax Court cases.
-   As Clerk of the Court, I need to ensure that only authorized Internal Court Users can view case records and filings in sealed cases.
-   As Clerk of the Court, I need to ensure that only permissible search results are available to the public so I don’t accidentally provide inappropriate information to unauthorized users.

#### Content Management

-   As an internal Court user, I need to be able to scan and upload paper documents so I can store and process them electronically.
-   As a Pro Se Petitioner, I need to electronically file documents so I can seek resolution of my dispute with the IRS.
-   As a Pro Se Petitioner, I need to file paper documents so I can seek resolution of my dispute with the IRS.
-   As a Member of the Tax Court Bar, I need to electronically file documents so I can seek resolution of the client’s dispute with the IRS.
-   As a non-party in a case, I need to electronically file various documents, such as amicus briefs, motions to quash subpoenas, notices of election to participate in a partnership case, or motions to intervene, so I can participate in an existing Tax Court case.
-   As an internal Court user, I need template orders and notices so I can streamline my work.
-   As an internal Court user, I need the ability to create unique orders and notices so I can properly address issues in a case.
-   As Clerk of the Court, I need to have codes associated with each type of court filing so I can track them in the System.
-   As an electronic filer, I need to attach documents for filing in my case so they can become part of the record.
-   As an internal Court user, I need to attach documents to orders and notices so they can become part of the record.
-   As an internal Court user, I need to see all user activity related to a case so I can monitor workflows.

## Location of Work to be Performed

The Contractor may choose the location(s) from which to perform the required software development services. All Tax Court Judges and staff are based at the Tax Court building at 400 Second Street, N.W., in Washington, D.C. The Court’s hours of operation are 8:00 a.m. to 4:30 p.m. Eastern Time. The Court’s Product Owner and any other necessary Court representatives will be available to confer with Contractor representatives on a daily basis during the development process, either in person at the Tax Court building or by video connection. In addition, the Court is willing to make space available on a daily basis for up to nine (9) Contractor representatives at the Tax Court building in Washington, D.C.

## Order Type and Ceiling Price

The Court intends to issue a time and materials task order under an existing contract under GSA Schedule 70, SIN 132-51, and all quotes must be submitted on that basis. The Court will not consider quotes that include fees for licenses or subscriptions. The Court will pay up to \$2 million for requested services and authorized travel incurred during the first year after the order, up to an additional \$2 million for services and authorized travel incurred during the first option year, and up to an additional \$2 million for services and authorized travel incurred during the second option year.

## Period of Performance

The period of performance shall be one year, with Court options to extend for up to two additional years. Services shall be provided, and expenses may be reimbursed for travel, during an initial period that begins with the date of the order and ends one year after the date of the order. The Court may, by written notice issued at least 15 days prior to expiration of the initial term, extend the period of performance for one additional year. If the Court exercises that option to extend the initial period of performance, the Court may also, by written notice issued at least 15 days prior to the expiration of that extended period of performance, again extend the period of performance for one additional year.

## Delivery Instructions

The Contractor must deliver all developed code to a GitHub repository designated by the Court on each day that the Contractor develops software code. The Contractor must also deposit documentation deliverables into a GitHub repository designated by the Court.

## Special Requirements

*Travel* – The Court will reimburse travel expenses necessary to provide the services required under the task order, up to a ceiling amount of \$50,000 per year, so long as each such expense is approved in advance by the Court. To be eligible for reimbursement, those travel expenses must be allowable under the General Services Administration Federal Travel Regulations in effect at the time the travel occurred.

*Key Personnel* – The Contractor must designate both a Project Manager (PM) and a Technical Lead as Key Personnel for this project. The PM will be a direct liaison to the Court product team, and will be responsible for the supervision and management of all of the Contractor’s personnel. The Technical Lead must have a full understanding of the technical approach to be used by the Contractor’s development team and will be responsible for ensuring that the Contractor’s development team follows that approach.

*Key Personnel Substitution* – Key Personnel substitutions must be approved by the Court in writing, and will only be justified by a Court request, sudden illness, death, change of employment, or termination of employment for cause. Contractor requests for a substitution of Key Personnel must include a detailed explanation of the justifying circumstances, and a complete résumé for the proposed substitute or addition, including skills, experience, education, training, and security level. The Court’s failure to approve a proposed substitution will not constitute grounds for non-performance by the Contractor, or form a valid basis for any claim for money or any equitable adjustment.

*Development Team Approval* – Each member of the development team proposed by the Contractor, including any subcontractors, must be approved in advance by the Tax Court before starting work. The Court may withhold approval, or at any time revoke a prior approval, for any reason. For each member of the development team proposed by the Contractor, the Contractor must provide the Tax Court with either a report generated within the last twelve (12) months from an Identity History Summary Check ([a technical fingerprint search of the criminal history records in the FBI national fingerprint database](https://www.fbi.gov/services/cjis/identity-history-summary-checks)), or an equivalent report or clearance acceptable to the Court.

*Teaming Arrangements* – Teaming arrangements, including joint ventures and subcontractors, are permitted with Court approval. The successful Offeror will be the prime contractor under this task order, regardless of any teaming arrangements, and must hold the Schedule 70 contract. The successful Offeror will be solely responsible for providing the required services, and payments will be made only to the successful Offeror.

*Data Rights and Ownership of Deliverables* – Consistent with FAR 52.227-14, which applies to this task order, the Court intends that all software and documentation delivered by the Contractor will be owned by the Court and committed to the public domain. This software and documentation includes, but is not limited to, data, documents, graphics, code, plans, reports, schedules, schemas, metadata, architecture designs, and the like; all new open source software created by the Contractor and forks or branches of current open source software where the Contractor has made a modification; and all new tooling, scripting configuration management, infrastructure as code, or any other final changes or edits to successfully deploy or operate the software.

To the extent that the Contractor seeks to incorporate in the software delivered under this task order any software that was not first produced in the performance of this task order, the Court encourages the Contractor to incorporate either software that is in the public domain, or free and open source software that qualifies under the Open Source Definition promulgated by the Open Source Initiative. In any event, the Contractor must promptly disclose to the Court in writing, and list in the documentation, any software incorporated in the delivered software that is subject to a license.

If software delivered by the Contractor incorporates software that is subject to an open source license that provides implementation guidance, then the Contractor must ensure compliance with that guidance. If software delivered by the Contractor incorporates software that is subject to an open source license that does not provide implementation guidance, then the Contractor must attach or include the terms of the license within the work itself, such as in code comments at the beginning of a file, or in a license file within a software repository.

In addition, the Contractor must obtain written permission from the Court before incorporating into the delivered software any software that is subject to a license that does not qualify under the Open Source Definition promulgated by the Open Source Initiative. If the Court grants such written permission, then the Contractor’s rights to use that software must be promptly assigned to the Court.

*Invoices* – Invoices for services and/or travel expenses must be submitted to the address (physical or e-mail) specified by the Court. To constitute a proper invoice, the billing document must include the following information and/or attached documentation:

\(1) Name of Contractor and Contractor’s Taxpayer Identification Number;

\(2) Period covered by invoice and invoice date;

\(3) Purchase order number;

\(4) All invoices for services must set forth in detail the following:

&nbsp;&nbsp;&nbsp;\(i) Individual performing service each day by hour and quarter of an hour;

&nbsp;&nbsp;&nbsp;\(ii) Type of services performed each day by hour and quarter of an hour; and

&nbsp;&nbsp;&nbsp;\(iii) Hourly rate for each service so detailed;

\(5) Any applicable payment discount terms; and

\(6) Total amount billed.

*Public Use of the Name of the Tax Court* – The Contractor may not publicly release any information pertaining to this task order without prior written approval from the Contracting Officer. The Contractor shall not refer to the Tax Court in advertising, news releases, brochures, catalogs, letters of reference, web sites, or any other media, in such a way as to represent or imply that the Court prefers or endorses the services offered by the Contractor, although the Contractor may refer to the Court as one of its customers when providing past performance information as part of a quote or proposal submission.
