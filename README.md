# 35_Agnt_LLM

Where QA needs to go in the era of agentic AI. 
AI and agentic test strategy: evaluating, adopting, and governing AI-assisted testing, 
autonomous test agents, and intelligent quality tooling
lead the shift to a modern automation strategy that embraces AI thoughtfully rather than reactively.

Success depends as much on people as on tooling. 
We need to influence across teams and seniority levels: 
building trust, explaining the why behind change, and bringing engineers and QA practitioners rather than imposing process from above. 
Accountable for this through defining, collecting, and reporting on quality metrics that demonstrate real outcomes, not just activity.

Leadership skills required (clear articulated point of view)
QA Engineer to QA Lead to Principal QA (leadership role) 
Line-managing direct reports across multiple teams 
Influencer:  Persuade, coach, and align engineers, squad leads, and Heads of Engineering behind a shared quality vision 
Leading process and/or tooling change across multiple teams 
Designing quality metrics and reporting on release/quality KPIs (e.g. change failure rate, deployment frequency, escape rate, test coverage) to senior engineering stakeholders 

AI & agentic testing (how AI and agentic tooling change the QA operating model — not just exposure to a tool, but experience evaluating, piloting, and governing its adoption) acroos the following areas: 
AI-assisted test generation, 
autonomous test agents, 
LLM-driven exploratory testing, 
AI-assisted triage

Technical skill  
Coding: Java, Python, C#, Robot-Framework
Test automation frameworks (Test automation UI & API) 
Test automation frameworks Selenium, Playwright, Cypress and BDD_Cucumber 
Git and CI tooling (e.g. Jenkins, TeamCity, CircleCI, GitHub Actions) 
Bug tracking and test case management tools (e.g. Jira, TestRail, Zephyr, qTest, PractiTest, or similar) 
BDD Cucumber and Agile methodoilogy (shift-left testing with built-to-fail approach)
ISTQB/ISEB certificate 

Infrastructure testing 
OSI layers
Non- functional performance testing
Upgrade and vulnerabilities: firmware/software/hardware upgrades and Penetration scanning
Mobile test automation frameworks (Appium) 
---------------------------------------------------------------------------
---------------------------------------------------------------------------

LLM-POWERED EXPLORATORY TESTING COPILOTS 
https://www.linkedin.com/pulse/llm-powered-exploratory-testing-copilots-narayanan-palani--5s36e/
Exploratory testing has always been the most valuable and least scalable thing testers do.
It depends on curiosity, domain memory, and the willingness to ask what happens if a copilot does not replace that instinct? 
It removes the blank-page problem (that wastes the first twenty minutes of every session) with extensive possible combinations to find useful bugs. 
It was TOUGH to run many exploratory tests in the past due to time crunch. 
Now LLMs are made for this demand!

WHY THIS MATTERS RIGHT NOW
Session-based testing produces enormous tacit knowledge that evaporates when the session ends. 
Language models are unusually good at capturing, summarising, and recombining that knowledge into charters the next tester can act on immediately.
The economics also changed. 
Historically, the cost of a thorough quality practice was measured in specialist hours, which meant depth was rationed and applied only to the highest-profile releases. 
Today the marginal cost of an additional analysis pass is small enough that depth can be the default rather than the exception. 
That inverts the old constraint. T
The question is no longer whether you can afford to test something thoroughly. 
It is whether you have designed a process capable of absorbing the volume of insight that thorough testing now produces without overwhelming the people responsible for acting on it.

KEY POINTS AT A GLANCE
----------------------
 1. Copilots are strongest at charter generation, oracle suggestion, and session note synthesis.
 2. Keep the human in control of navigation; let the model propose risks, not decisions.
 3. Feed the copilot production incident history so suggestions reflect real failure modes.
 4. Structured session notes turn exploratory findings into durable regression assets.
 5. Time-boxed charters prevent an infinite suggestion loop from consuming the session.
 6. Debriefs improve faster when the copilot drafts the summary and the tester corrects it.

WHY THE OLD PLAYBOOK BREAKS HERE
--------------------------------
Most quality processes were designed for a world where requirements arrived before code and code arrived before testing. 
That sequence has effectively collapsed. 
Requirements evolve during implementation, models change after deployment, 
and user behaviour reshapes the system through feedback loops that nobody explicitly designed. 
Testing as a phase cannot survive that environment. 
Testing as a continuous property of the system can.

The practical consequence is that this practice, LLM-powered exploratory testing copilots, 
has to be embedded rather than scheduled. 
It runs inside the pipeline, inside monitoring, and inside the decision-making rituals of the team. 
When it lives outside those places, as a document produced before a release, it describes a system state that expired before anyone read it.
There is also a cultural shift underneath the technical one. 
When quality signals are continuous, the conversation changes from did we pass to are we improving. 
That framing is significantly healthier for engineering teams, because it replaces a pass or fail verdict delivered late with a trend that everyone can influence early.

HOW TO PUT THIS INTO PRACTICE
-----------------------------
The implementation path below assumes you have limited time, existing commitments, and a backlog that already looks intimidating. 
That is the normal condition of every engineering team, and any practice that requires ideal circumstances will never be adopted. 
Each step is designed to produce something useful on its own, so if you stop after step two you still keep the value you have earned.
 Step 1 - Define a charter template with mission, risk area, data preconditions, and stop conditions.
 Step 2 - Prime the copilot with recent defects, architecture notes, and the current release scope.
 Step 3 - Run a ninety-minute session where the copilot proposes three alternative attack angles at each dead end.
 Step 4 - Capture screenshots and observations continuously, then ask the copilot for a structured debrief.
 Step 5 - Convert the highest-value findings into automated regression checks before the session context fades.

TOOLS, PLUGINS, AND REFERENCES WORTH EXPLORING
----------------------------------------------
Choose tools the way you would choose a dependency, because that is what they are. 
Prefer open standards where the data is valuable, 
Prefer managed platforms where the operational burden is high, and always confirm you can export your evidence if you change vendors. 
The following references are grouped into specialist tooling for this practice and the broader ecosystem that supports AI quality work generally.

Specialist tooling for LLM-powered exploratory testing copilots:
 - Playwright Trace Viewer (https://playwright.dev/docs/trace-viewer) - replay exploratory paths with full context.
 - BrowserStack (https://www.browserstack.com) - broaden exploratory reach across real devices and browsers.
 - Java Surefire reports & Allure Report (https://allurereport.org) - structure session evidence into readable, shareable output.
 - ReportPortal (https://reportportal.io) - aggregate findings and cluster related failures across sessions.
 - mabl (https://www.mabl.com) - low-code capture of exploratory paths into repeatable journeys.
 - Sentry (https://sentry.io) - pull real production error signatures into charter planning.

Cross-cutting tooling every AI quality team should know:
 - pytest (https://docs.pytest.org) - the assertion and fixture backbone for most Python-based quality tooling.
 - Playwright (https://playwright.dev) - reliable end-to-end automation with tracing and parallel execution.
 - GitHub Actions (https://github.com/features/actions) - pipeline orchestration for continuous quality gates.
 - Testcontainers (https://testcontainers.com) - disposable, reproducible dependencies for isolated test runs.
 - OpenTelemetry (https://opentelemetry.io) - vendor-neutral instrumentation across services and AI pipelines.
 - Langfuse (https://langfuse.com) - open-source tracing, evaluation, and scoring for LLM applications.

Standards and reference material:
 - OWASP GenAI Security Project (https://genai.owasp.org) - the reference risk taxonomy for LLM applications.
 - NIST AI Risk Management Framework (https://www.nist.gov/itl/ai-risk-management-framework) - structured governance language.
 - ISO/IEC 42001 (https://www.iso.org/standard/81230.html) - management system requirements for AI.
 - ISTQB Certified Tester AI Testing (https://www.istqb.org/certifications/artificial-inteligence-tester) - shared vocabulary for AI quality.

 - Google SRE Workbook (https://sre.google/workbook/table-of-contents) - practical reliability engineering patterns.

METRICS THAT PROVE IT IS WORKING and GET YOU IMPORTANT ROLE IN QA ROLES
--------------------------------
Measure outcomes rather than activity in Copilot Testing. 
The number of tests written, prompts evaluated, or scans executed tells you how busy the team was, not whether the product improved. 

The metrics below are deliberately weighted towards detection, prevention, and speed of feedback, 
because those are the properties that customers eventually experience. 
Track a small set consistently, and resist adding new indicators until an existing one has changed a decision at least once.
 - Unique defects found per session hour.
 - Percentage of exploratory findings converted into automated checks.
 - Charter coverage across risk areas per release.
 - Time spent on session setup versus actual exploration.
 - Repeat-defect rate in previously explored areas.
---------------------------------------------------------------------------
---------------------------------------------------------------------------

REPORTING:
Maven Surefire Report
• Role: Executes unit tests in a Maven build and outputs basic test results (XML and plain text files).
• Report Quality: Minimal, plain, and text- or basic-HTML-based.
• Features: Focuses on functional pass/fail status and stack traces for CI/CD pipeline gates.
• Setup Effort: Near zero; it runs automatically during mvn test when configured in your project.

Allure Report
• Role: Takes raw test outputs (including JUnit, TestNG, or Cucumber) and transforms them into a rich, modern, stakeholder-ready dashboard.
• Report Quality: Highly polished, interactive, and visual.
• Features: Includes step-by-step test breakdowns, severity levels, issue tracker links, historical trend graphs, screenshots/attachments, and categorization of failures (product defect vs. test script defect).
• Setup Effort: Medium; requires adding language-specific Allure listeners/adapters and using the Allure CLI or CI action to render the final report.

Use both together: Surefire handles execution and basic XML output for CI/CD build status, while Allure consumes those results to generate rich HTML dashboards for humans.
For a Project, first look at:
• What testing framework (JUnit 5, TestNG, Cucumber, etc.) you are using
• Whether you need this for local developer feedback or CI/CD pipelines (like GitHub Actions or Jenkins)
Use AI to help configure the right plugin setup.
