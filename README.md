<h1>Hi, I'm Nate! <br/><a href="https://YOUR-USERNAME.github.io">Accounting &amp; Data Analytics Student</a>, <a href="https://www.linkedin.com/in/natnael-tecle/">Future Auditor</a>, <a href="https://YOUR-USERNAME.github.io/projects.html">Problem Solver</a></h1>
I turn messy financial data into answers an auditor can trust.

I'm a Master of Accountancy student at the University of Denver's Daniels College of Business, combining audit and forensic accounting training with hands-on data skills in Python, SQL, and Alteryx. I'm looking for roles in audit, forensic accounting, or accounting data analytics where I can test controls and also automate the testing. I was born and raised in Colorado.

👉 Visit my full portfolio site

	
Education	MAcc (March 2027, GPA 3.56) and BS in Accountancy (June 2026, GPA 3.31), University of Denver
Technical toolkit	Python (ARIMAX forecasting), SQL, Alteryx, advanced Excel (certified)
Professional network	Beta Alpha Psi member since 2024
Target roles	Audit, forensic accounting, accounting data analytics
Contact	720-589-9662 · natnael.tecle@du.edu · LinkedIn
🧰 Skills
Technical

Python — Forecasting, data analysis, and app building I used Python to build an ARIMAX time-series model that forecasts Starbucks quarterly revenue, with CPI as an outside input and average ticket as an added variable. The model produces a forecast with a confidence band. I wrapped it in a Streamlit app that pulls live CPI data from FRED, accepts a user assumption, flags quarters where actual revenue runs above the forecast range, and produces an AI-assisted summary written for an audit committee. The hard parts were lining up data series with different frequencies and explaining the method in plain language to a non-technical audience. I also use loops and flowcharts to plan program logic before writing code.

<img src="images/starbucks-forecast.png" alt="ARIMAX forecast of Starbucks quarterly revenue with confidence band and average ticket" width="700"><br/> <sub>ARIMAX revenue forecast with CPI input and average ticket trend.</sub>

SQL — Querying, aggregating, and designing relational databases Querying: I use SQL to turn tables into answers. I join multiple tables and summarize with COUNT, SUM, AVG, MIN, and MAX. I know the difference between COUNT(*) and COUNT(column), since NULL values change the result. I use GROUP BY to total amounts by customer or state, and HAVING to filter on those totals, for example to find states whose orders exceed a dollar threshold. I filter early with WHERE when I can, so the database groups less data, and I use subqueries to compare values against an overall average. Design: I designed a five-table database for a landscaping company, with primary and foreign keys and an associative table to resolve a many-to-many relationship. In audit work, the same skills support reconciliation and testing whole populations instead of samples.

<img src="images/coastline-erd.png" alt="Entity relationship diagram with Client, Invoice, Property, Property Service, and Service tables" width="700"><br/> <sub>Entity relationship diagram for the Coastline database.</sub>

Alteryx — Data preparation, reconciliation, and business analysis I completed an individual data consulting project for Eddie's Tennis Warehouse, a wholesale tennis equipment distributor, covering a full year of its sales-to-cash process. I loaded multiple files (invoices, customers, cash receipts, product list, and sales team data), cleansed them, and tied each one to the client's control totals before any analysis, so the results could be trusted. I then built workflows to examine management's concerns, including whether the reported accounts receivable balance of $590,738.64 was supportable, whether customers stayed within credit limits, which invoices were more than 90 days old and might need write-offs, whether early-payment discounts followed policy, whether sales reps used official retail prices, and what commissions would cost. For each result, I wrote up what it meant for the business, not just the numbers, in a client-ready report.

Microsoft Office — Certified: advanced Excel, Word, PowerPoint Pivot tables, VLOOKUP, conditional formatting, charts, and presentation design for financial reporting.

Professional
Attention to detail under rules: Documented meal orders accurately for memory care residents, where dietary requirements were non-negotiable. The same habits carry into audit work.
Communication and teamwork: Worked across departments at Modena, collaborated on the Madden Innovation Challenge, and organized service events through Beta Alpha Psi.
📊 Projects
AI-Powered Revenue Forecasting App for an Audit Committee

ITEC 3155 / ACTG 4155 · Spring 2025 · Python, Streamlit, ARIMA/ARIMAX · Partner project, presented in a group of four

Business problem: Auditors need early warning when a company's reported revenue looks too good. This project asked: how can an audit committee evaluate the risk that Starbucks has overstated revenue, using a forecast as the benchmark?
My role: I built the forecasting engine and the data pipeline. That included fitting the ARIMAX model from my earlier project, pulling live CPI data from FRED, and connecting both to a user input for expected revenue growth. My partner focused on the page layout and charts, and we split the AI summary and the written documentation.
New insight: I added average ticket (the average amount spent per transaction) as the new variable, plotted beside revenue. It let us ask whether revenue growth came from customers spending more per visit or from more visits.
Challenges: The live CPI data arrived in a different frequency than quarterly revenue, so I had to align the two series before the model would run. Early AI summaries were too generic for an audit committee, so I rewrote the prompts to require specific numbers and a clear risk statement, then edited the output by hand. I also had to explain ARIMA without jargon.
Enhancement: Risk-flagging logic that marks a quarter when actual revenue sits well above the forecast range, so the committee sees where to look first.
Business value and outcome: Revenue climbed steadily from 2018 to 2024 while average ticket drifted down and swung more widely, which suggests growth came from more transactions rather than higher prices per visit. That is the pattern an audit committee should test against store count and traffic data before accepting the forecast as a clean benchmark, so we presented it as a moderate-risk finding. The app turns a statistical model into a risk signal a non-technical committee can read in one chart and one message.

<img src="images/starbucks-forecast.png" alt="ARIMAX forecast of Starbucks quarterly revenue with confidence band and average ticket" width="700"><br/> <sub>ARIMAX forecast of Starbucks quarterly revenue with CPI as an input. The blue line is observed revenue, the dashed orange line is the forecast, and the gray band is the confidence interval. The purple line is average ticket on the right-hand axis, the new variable I added. The forecast puts revenue near $9.0 billion per quarter through 2025, within a band of roughly $8.4 to $9.7 billion.</sub>

IT Audit and Cybersecurity Readiness Assessment: Fast Freddy's Furniture Depot

ACTG 4575 · Team simulation of a client engagement · Audit program, workpapers, findings, and executive presentation

Business problem: Fast Freddy's, a Denver furniture manufacturer with a growing web business, runs everything on one SAP ERP system hosted in an Omaha datacenter. Executives wanted to know how ready their cybersecurity was, and the financial statement auditors needed to know whether they could rely on the company's IT general controls.
My role: I helped draft the audit program before our interview with the CIO and took the lead on the user account management and password settings sections, from test steps through workpapers. I also helped write up findings and presented the access control results to the client's executives.
Challenges: Interview time and follow-up requests were limited, so we prepared a draft audit program and a question list in advance and used only our allowed follow-ups. We also had to fold in the datacenter and backup results from another audit team so the program and findings read as one engagement.
Business value and outcome: Using the NIST Cybersecurity Framework as our rating scale, we rated Govern, Detect, and Respond as high risk and Identify, Protect, and Recover as medium. Our top recommendations were a formal incident response plan with a ransomware tabletop exercise, restoring the intrusion detection capability with continuous log monitoring, and documented governance roles. In the IT audit, findings included user accounts that stayed active after employees left, password settings weaker than company policy, and program changes without documented approval. We concluded that the audit team could not rely on the IT general controls this period without expanded substantive testing, and we gave management a prioritized list of fixes, starting with access removal.

<img src="images/cybersecurity-readiness.png" alt="Table rating six cybersecurity functions as high or medium risk, each with a recommended action" width="700"><br/> <sub>Cybersecurity readiness results, organized by the six functions of the NIST Cybersecurity Framework. Govern, Detect, and Respond were rated high risk, and Identify, Protect, and Recover medium risk. Each row pairs the rating with a specific recommendation, such as a formal incident response plan, restoring the intrusion detection system, and tested backup recovery.</sub>

Coastline Landscaping Database Design

INFO 3140 · SQL, entity relationship modeling · Individual project

Business problem: Coastline, a growing West Coast landscaping company, spread its resources too thin across several states. Management wanted to find its most and least popular services, identify the regions with the highest demand, and focus on smaller markets before restructuring the business.
My role: I did all of it: wrote the business rules, designed the five-entity model (Client, Invoice, Property, Service, and Property Service), drew the ER diagram in Lucidchart, built and loaded the database in SQL, and wrote the queries. Because properties and services are many-to-many, I resolved that relationship with the Property Service table.
Challenges: Keeping the ER diagram and the actual tables consistent, getting cardinality right, and making sure every foreign key pointed to a real primary key. The many-to-many relationship was the part I had to rework before the design was correct.
Queries: Four queries, each with a business purpose: services ranked by the number of properties served; clients whose total billing exceeded a threshold (GROUP BY with HAVING); properties with no services recorded, using an outer join; and revenue by region.
Business value and outcome: The queries showed that a few core services, such as irrigation maintenance, drove most of the activity, while specialty services like pest control were requested far less often. That is the evidence management needs to decide which offerings to strengthen and which to phase out.

<img src="images/coastline-erd.png" alt="Entity relationship diagram with Client, Invoice, Property, Property Service, and Service tables" width="700"><br/> <sub>Entity relationship diagram for the Coastline database. A client has many invoices and many properties. Properties and services have a many-to-many relationship, resolved by the Property Service table, which holds the service date. Every table has a primary key, and each foreign key points to a primary key in another table.</sub>

What these projects have in common

The forecasting app tests whether reported numbers look reasonable, the IT audit tests whether the systems producing those numbers can be trusted, and the database shows I can organize the data in the first place.

💼 Work Experience
Server, Modena Cherry Creek Senior Assisted Living

Denver, CO · October 2021 to June 2023

What I did: Processed and documented resident meal orders accurately, coordinating across departments so service stayed on time and met dietary and care requirements, including memory care units. Organized and monitored the dining room and servery across three floors.
Soft skills: Attention to detail, professional communication with residents, management, and staff, and working in a regulated care environment.
Connection to accounting: Documentation accuracy and following controls are the same habits audit depends on.
🎓 Education
Master of Accountancy

University of Denver, Daniels College of Business · March 2027 · GPA 3.56

Consolidated Financial Statements: Combining parent and subsidiary results, eliminating intercompany transactions.
Topics and Cases in Managerial Accounting: Using cost and performance data to support management decisions.
Accounting Information System Risk, Control and Audit: Evaluating IT controls and risk in accounting systems.
Forensic Accounting and Auditing: Detecting and investigating fraud.
Corporate and Partnership Taxation: Tax treatment of corporations and partnerships.
Bachelor of Science in Accountancy

University of Denver · June 2026 · GPA 3.31

Intermediate Financial Accounting I, II, III: Financial reporting under GAAP.
Cost Management and Managerial Accounting: Costing, budgeting, and variance analysis.
Auditing: Audit evidence, risk, and reporting.
Business and Investment Tax Issues: Tax planning for businesses and investments.
Accounting Data Analytics and Data Skills & Concepts: Python, SQL, and Alteryx applied to accounting data.
🏔️ Beyond Class

I was born and raised in Colorado, and a lot of how I work comes from growing up here: show up early, be prepared, and don't mind a little hard work to get to a good view.

Beta Alpha Psi (member since 2024): National honors organization for accounting, finance, and information systems. I attended firm presentations, technical workshops, and networking events with accounting professionals, and took part in a holiday outreach event, preparing and organizing gift bags for children. The experience built my communication, professionalism, and ethical conduct for public accounting and corporate finance.
Hiking and camping: Weekend trips to the mountains, from easy trails to early-morning climbs. Planning gear, weather, and timing before a hike is good practice for planning an audit.
Skiing and snowboarding: Winters mean time on the slopes, and learning to keep going after a fall is a lesson that carries over to busy season.
Cheering for Denver teams: Broncos, Nuggets, and Avalanche games. Sports fans love statistics, and I'm no exception.
Exploring Denver: Trying new restaurants, parks, and neighborhoods in the city I've always called home.
🤳 Connect with me

<img align="left" alt="Nate Tecle | LinkedIn" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/linkedin.svg" />

📫 Email: natnael.tecle@du.edu · 📞 720-589-9662
