# About Me

## Who I Am

- **Name:** David Tunnell
- **Role:** Lead Software Architect at [Webapper Services, LLC](https://www.webapper.com/)
- **Location:** Castroville, Texas just outside of San Antonio
- **Education:** University of Maryland University College - Bachelor of Computer Science - Cum Laude | Master of Business Administration - MBA | The University of Texas at Austin (2010–2013)
- **Portfolio:** [GitHub](https://github.com/DavidTunnell) | [Stack Overflow](https://stackoverflow.com/users/1524210/david-tunnell) | [Linkedin](https://www.linkedin.com/in/david-tunnell/)

## What I Do Day-to-Day

I'm a software architect at Webapper Services, a web development and consulting company. My work spans both technical leadership and business strategy:

- **Architecture & Design:** I design system architecture for client projects and internal products. I make technology decisions, define patterns, and ensure quality across the codebase.
- **Agile Coaching:** I run Scrum ceremonies, coach teams on agile practices, and maintain project health. I hold a Certified Tactical Agilist certification and SAFe SPC experience.
- **Requirements & Planning:** I write and manage requirements in Jira and Productboard, translating business needs into actionable technical work.
- **AI Transformation:** I'm leading Webapper's transformation into an AI-native company — this is my top strategic initiative. We're going Anthropic-first with Claude Desktop, Claude Code, Claude Cowork, and Anthropic platform API calls. The vision is a full adoption roadmap: get the whole team on the tools, train everyone on effective LLM prompting and workflows, build and deploy agents that automate repetitive tasks, and stand up a central agent dashboard where every deployed agent is visible, monitored, and managed. The goal isn't to replace developers — it's to empower each person on the team to ship more, faster, and tackle work that would have been out of reach before. Long-term, the default for any new feature, project, or process should be "how can AI help us build this faster and better?" I wrote and delivered an internal AI manifesto to the team laying out this vision and the concrete steps to get there.
- **Path to CTO:** I'm actively working toward a CTO role, which means I'm balancing hands-on technical work with strategic leadership, team development, and company-wide technology decisions.

## Primary Tech Stack

- **Frontend:** React, TypeScript, JavaScript
- **Backend:** Node.js, TypeScript
- **Cloud:** AWS (S3, Lambda, MySQL or DynamoDB in RDS and broader serverless patterns)
- **Tools:** Jira, Productboard, GitHub, VS Code, Docker, Claude Code, Claude Desktop, Windows, Google Workspace, Atlassian Suite
- **Methodologies:** Scrum, Agile Coaching

## Team Structure

**US Team:**
- **Patrick Quinn** — CEO (pquinn@webapper.com)
- **Scott Herring** — COO / Marketing / Sales / SEO (scott@webapper.com)
- **Joy Miller** — Technical PM, Scrum Master, Manual Tester, SME of VisionAST (joy@webapper.net)
- **Daniela Camargo** — PM, Scrum Master, Manual Tester, SME of CloudSee (daniela@webapper.net)
- **David Tunnell (me)** — Lead Software Architect (david@webapper.com)

**Vietnam Team (VTeam):**
- **Steven** — Tech Lead, all projects
- **Ann** — Sr. Dev, VisionAST
- **Peter** — Sr. Dev, CloudSee Drive (also helps with VisionAST onboardings)
- **Kevin** — Sr. Dev, transitioning from EDS contract into AI initiative
- **Henry** — SDET, Documentation, Selenium, Unit Tests, DevOps
- **Max** — Jr/Mid Dev, CloudSee Drive

## Our Product — CloudSee Drive

Webapper's top product is [CloudSee Drive](https://www.cloudseedrive.com/), a SaaS platform that gives teams a user-friendly browser-based interface for Amazon S3 storage. It lets AWS administrators and end users browse, search, upload, download, and manage files across S3 buckets without needing the AWS Console or technical expertise. Key capabilities include sub-second search across millions of objects (Fast Buckets indexing), file versioning, RBAC permissions management, secure file sharing via time-limited links, activity monitoring and audit logs, and support for files up to 5TB. It's available through the AWS Marketplace with same-day onboarding. Revenue is currently low, but the strategic goal is for CloudSee Drive to replace client services revenue and become Webapper's primary business.

**CloudSee Drive Tech Stack:**
- **Frontend:** React, hosted on S3 + CloudFront CDN (repo: Bitbucket `csd-frontend`)
- **Backend:** Node.js microservices deployed as AWS Lambda functions via SAM CLI / CloudFormation. Services include: User API, Storage API, Metric Service, Fast Bucket Service (indexing engine), Task Manager, and Zipper Task. Shared SDK (`@webapper/cloudsee-drive-sdk`) on NPM handles DB connections, CORS, and auth. (repo: Bitbucket `csd-backend`)
- **Database:** DynamoDB (tables prefixed by environment, e.g. `production_User`)
- **Search:** OpenSearch (powers Fast Buckets indexing; AI-powered natural language + voice search in development)
- **AWS Services:** S3, Lambda, API Gateway, CloudFront, DynamoDB, OpenSearch, SES (email), Systems Manager Parameter Store, CloudFormation
- **Auth:** SSO-ready, Microsoft Entra ID integration for group management
- **Environments:** Develop → QA → Production, all in us-east-1
- **Primary devs:** Peter (Sr. Dev), Max (Jr/Mid Dev), Daniela (PM/SME)

## Client Project — VisionAST

[VisionAST](https://www.visionast.com/) is Webapper's primary client project — a data analytics platform built for automotive and powersports dealerships. It helps dealers unlock profitability through real-time reporting on their DMS (dealership management system) data. The product suite includes SalesVision (variable ops reporting), PowerVision (powersports-specific), FinanceVision (F&I analytics), ServiceVision (service department metrics), and MenuVision (F&I video/reporting via iTapMenu partnership). It integrates with 12+ DMS systems, runs on AWS, and provides unified single sign-on access across multi-location dealer groups. Joy Miller is the SME and PM on this project, with Steven and Ann as the primary devs.

## AWS Hosting Customers

Webapper also provides AWS hosting services for several clients:

- **[Atlantic British / RoverParts](https://www.roverparts.com/)** — Specialized retailer for Land Rover and Range Rover parts and accessories, with 11,000+ parts across two US warehouses.
- **[Icon Media](https://www.icon-media.com/)** — Full-service advertising agency in Anaheim Hills, CA specializing in the automotive aftermarket industry, including their iConfigurators visual software.
- **[eRep](https://erep.com/)** — Psychometric assessment platform offering the Core Values Index (CVI) for hiring and employee engagement.

## Other Client Work

- **[Educational Data Services (EDS)](https://www.ed-data.com/)** — Cooperative procurement platform for schools and public entities. Webapper was modernizing their systems (Azure-based). Relationship ending after ~2.5 years; Kevin is transitioning off this contract.

## Current Priorities

1. Leading AI transformation at Webapper Services
2. Architecting and shipping client projects
3. Building AI first systems and processes that scale as I move into a CTO role. Replacing company processes with standardized agents across the company.
4. Staying sharp on full-stack development using Claude Code while expanding leadership scope

## What I Care About

- Clean, maintainable architecture over clever hacks
- Teams that ship reliably through good process
- Practical AI adoption — tools that actually save time, not hype
- Clear communication between technical and non-technical stakeholders