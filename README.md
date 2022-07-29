<p align="center"> <strong>Star this repo and keep track of awesome new updates.</strong> </p>

![Banner](./img/Banner.png)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) ![GitHub last commit](https://img.shields.io/github/last-commit/h-parikh/awesome-dev-first-security) ![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fh-parikh%2Fawesome-dev-first-security%2F) 


> A curated collection of tools and resources for building security with a developer first mindset.

Security with a dev-first mindset brings security closer to developers, empowering them to take ownership of security. This democratization of security changes the role of security teams to be an enabler rather than controller, and requires developers to embrace security as a first class citizen.

Your [contributions](https://github.com/h-parikh/awesome-dev-first-security/blob/main/contributing.md/) are always welcome !

# Contents
- [Secure Development](#secure-development)
- [Continuous Security Testing](#continuous-security-testing)
- [Triage and Prioritizaiton](#triage-and-prioritization)
- [Remediation Management](#remediation-management)
- [Metrics and Reporting](#metrics-and-reporting)
- [Training](#training)

![Lifecycle](./img/Lifecycle.png)

## Secure Development
Building security from the beginning is well accepted as the ideal goal, however it is incredibly hard to implement in practice. In a constantly changing landscape of security, it is not practical to expect every single developer to follow security practices all the time. In most organizations, where developers are at varying levels of security skills and have constantly changing priorities, it becomes important to make security simple to follow and difficult to get wrong. This is where checklists come into the picture. Building out well defined, actionable checklists and implementing those checks technically is known to significantly improve the security posture of software being built by developers. Here are a few usable checklists:
- [OWASP ASVS](https://github.com/OWASP/ASVS/)
- [Mozilla’s Web Security Checklist](https://github.com/mozilla-services/websec-check/)
- [Test Driven Security in CI](https://www.youtube.com/watch?v=e2axToBYD68/)
- [API Security Checklist](https://github.com/shieldfy/API-Security-Checklist/)
- [Case studies of successfully eliminating entire classes of vulnerabilities](https://docs.google.com/presentation/d/1neDK74PT-y2zt-nOV0fN80m0TJeoBRp9iVZp8R78Jbg/edit#slide=id.g2baad2bc301217d9_10/)
- [Making safe coding patterns the default](https://www.slideshare.net/morganroman/banfootguns-devseccon-2019/)
- [Serverless security checklist](https://res.cloudinary.com/snyk/raw/upload/v1559295122/Cheat_Sheet-_10_Serverless_Security_Best_Practices.pdf)

Note: The problem of avoidable failures is not limited to security or development, in fact it is prevalent in almost every organized activity including healthcare, airlines, government etc. An excellent book to read on the importance and impact of checklists is [The Checklist Manifesto](https://amzn.com/0312430000/)

## Continuous Security Testing
DevOps practices have introduced continuous integration (CI) which puts focus on continuously testing code during the development process. Following a similar pattern, making security verification an integral part of development process typically leads to security becoming more actionable and natural for developers to work on. Here are a few tools and resources for security testing throughout the development and deployment lifecycle:
- Orchestrate scanners in CI/CD - [ReapSaw](https://github.com/dowjones/reapsaw/) and [Salus](https://github.com/coinbase/salus/)
- Orchestrate security using AWS step functions - [Slides](https://www.deepsec.net/docs/Slides/2018/Orchestrating_Security_Tooling_With_AWS_Step_Functions_Jules_Denardou_Justin_Massey.pdf/)
- GitHub app for security feedback in PRs - [GuardRails](https://github.com/apps/guardrails/)
- Static analysis for Infrastructure as Code - [Checkov](https://github.com/bridgecrewio/checkov/)
- Open source static analysis tool - [InsiderCLI](https://github.com/insidersec/insider/)
- [More Scanners](https://github.com/devsecops/awesome-devsecops#automation/)
- [Awesome BugBounty](https://github.com/djadmin/awesome-bug-bounty/)
- [Awesome Pen Testing](https://github.com/enaqx/awesome-pentest/)
- [Awesome Threat Modeling](https://github.com/redshiftzero/awesome-threat-modeling/)
- [Awesome Web Hacking](https://github.com/infoslack/awesome-web-hacking/)
- [Awesome Container Security](https://github.com/kai5263499/awesome-container-security/)
- [Building a Secure DevOps Pipeline](https://www.youtube.com/watch?v=IAzPKzwY-ks/)

## Triage and Prioritization
Security tools, especially automated scanners are notorious for generating high ratios of false positives. The easiest way to lose developers' attention and interest in security is by sending them on a wild goose chase of highly noisy vulnerability report. While this problem of high rate of false positives is still not solved, several folks are trying to solve this problem in different ways. Here are a few tools and resources that are helpful in triaging and prioritizing vulnerabilities:
- Vulnerability intelligence services to prioritize CVEs - [vFeed](https://vfeed.io/) and [Vuldb](https://vuldb.com/) and [VulnDB](https://vulndb.cyberriskanalytics.com/)
- Research study for using ML in improving vulnerability identification - [Article](http://asankhaya.github.io/pdf/Effective-Identification-of-Vulnerabilities-using-Machine-Learning.pdf/)

This focuses on network vulnerabilities but several concepts can be borrowed in AppSec world 
- [Collective intelligence for contextual prioritization](https://delvesecurity.com/contextual-prioritization-score/)
- [Remediation Prioritization](https://delvesecurity.com/re-defining-vulnerability-remediation-prioritization/)
- [Threat Intelligence for Prioritization](https://delvesecurity.com/automating-threat-intel-with-machine-learning-extracting-the-underlying-concepts-from-underground-discussions-and-osint/)

## Remediation Management
Dealing with security defect backlog and getting it prioritized for remediation can be a constant challenge in most organizations. A dev-first approach to this challenge brings empathy and partnership into the mix, and puts security team in the role of an enabler rather than a controller. Here are a few excellent case studies of security and engineering partnerships:
- Building partnerships and enabling engineers - [Abstract](https://tldrsec.com/blog/appsec-cali-2019/#a-pragmatic-approach-for-internal-security-partnerships/) and [Original Video](https://www.youtube.com/watch?v=HIdexRqjpWc/)
- Art of Vulnerability Management - [Abstract](https://tldrsec.com/blog/appsec-cali-2019/#the-art-of-vulnerability-management/) and [Original Video](https://www.youtube.com/watch?v=EkyY1q2-JBI/)

## Metrics and Reporting
Generating metrics for the overall AppSec program or vulnerability management program is important, however that will not necessarily move the needle with developers. A dev-first approach to AppSec metrics, is to bring visibility to each dev team of their own AppSec performance metrics and have them take ownership of it. Just like how dev teams measure their quality, reliability, performance metrics, they should be able to measure and improve their own AppSec metrics. Here are a few resources that can help you get started: 
- Simple AppSec Metrics - [Abstract](https://tldrsec.com/blog/data-driven-bug-bounty/) and [Original video](https://www.youtube.com/watch?v=2TWY74MgTrc/)
- More Metrics - [Original Video](https://youtu.be/BxXV1pVSMn0?t=1751/)
- Building Actionable KPIs - [Slides](https://published-prd.lanyonevents.com/published/rsaus20/sessionsFiles/18075/2020_USA20_RMG-F02_01_beating-security-inertia-with-actionable-KPIs.pdf)
- Vulnerability Aggregation Tool - [DefectDojo](https://github.com/DefectDojo/django-DefectDojo/)
- Dashboarding Tools - [Metabase](https://github.com/metabase/metabase/), [Superset](https://github.com/apache/incubator-superset/)

## Training
In security, failures (bugs / defects / vulnerabilibities) are caused by not just lack of security skills. In a large majority of the cases, security defects are caused by competent developers who have too many other priorities or are not incentivized to build security or simply don't connect the dots to security risks. To address such a broad set of failure modes, security training needs to go beyond a focus on skills improvement and needs to also include things that make security interesting, fun and engaging. Building out a security champions program, organizing CTFs and gamifying the experience have led to increased developer engagement and interest towards security.
- [Security Champions Playbook](https://github.com/c0rdis/security-champions-playbook/)
- [Awesome CTF](https://github.com/apsdehal/awesome-ctf/)
- [Awesome AppSec](https://github.com/paragonie/awesome-appsec/)
- [Awesome Cyber Skills](https://github.com/joe-shenouda/awesome-cyber-skills/)
- [SecDim - Learn appsec the fun way](https://secdim.com)



