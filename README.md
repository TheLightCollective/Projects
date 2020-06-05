# SuperFunProject

## Open Source Solutions for getting Peer Support Groups off of Facebook

* [Community Slack channel: LightCollective](https://lightcollective.org/) via an [open invite link](https://join.slack.com/t/thelightcollective/shared_invite/zt-e1wc5c91-mKCTttExywUu~4Mgeu9jIg)

* [Meetings: Google calendar](https://calendar.google.com/calendar?cid=YnJhdmVib3NvbS5vcmdfNjl1OWp2dmpua2lqbzk1dHE1azUyMThhYW9AZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ)

* Project Trackers: [Core](https://github.com/TheLightCollective/SuperFunProject), 
[Interventions](https://github.com/TheLightCollective/SuperFunProject), and [Issues](https://github.com/TheLightCollective/SuperFunProject)



## Data

We are collecting, analyzing, and sharing data around:

* COVID Twitter: Who is saying what and when, including around URLs
* Feeds: Correlations against labeled data such as bots, fact checks, and indicators of digital crime  
* Scores: Bots, misinformation, crime, likely location, and more


## The interventions

We are working with ethics groups to identify safe interventions along the following lines:

* **Alert individuals as they are being manipulated**: For manipulated conversations where we have clear intelligence, we are exploring an alert bot that will post the misinformation report directly on the thread, or enable community participants or project partners to do so.

* **Enable other platforms**: We expect a growing number of initiatives to benefit from our intelligence and automation capabilities.

## The technologies

* See Slack

## How to help

We are actively seeking several forms of support:

* **Volunteers**: Most immediate priority is on data engineering and advisors on marketing/public health
  * **Data engineers: Orchestration (Airflow, Prefect.io, Nifi, ...), streaming (Kafka, ...),  graph (Neo4j, cuGraph), GPU (RAPIDS), ML (NLP libs), and databases**
  * **Analysts: OSINT, threat intel, campaign tracking, ...**
  * **Data scientists: especially around graph, misinformation, neural networks, NLP, with backgrounds such as security, fraud,  misinformation, marketing**
  * Developers & designers: intelligence integrations, website for search & reports, automations, intervention bots, API
  * Marketing: Strategy & implementation
  * Public health and communications: Especially around safe and effective intervention design
  * Legal: Risk & legal analysis for various interventions

* **APIs and Data**: 
  * Feeds & enriching APIs: Lists and intel on URLs, domains, keywords, emails, topics, blockchain accounts, social media accounts & content, clinical trials, esp. if tunable on topic
  * Scoring: Libraries and APIs around social networks (initially Twitter) structure & content, websites, and news: bot scores, fingerprinting, topic extraction & classification
  * Crawling tech: Social networks and web

* **Software Licenses**:
  * **SaaS, OSS, Docker preferred**
  * Project management
  * Analytics
  * Automation

* **Hardware**: Anything you can provide along the lines of:
  * 1 x Database server (CPU): 32+ cores, Ubuntu 18, 64GB+ RAM, ideally backups
  * 1 x Primary analytics server (GPU) - 32+ CPU cores, 128GB+ CPU RAM, 2-8 GPUs, 64GB+ disk, 2-10TB attached SSD
    * GPUs: Nvidia Pascal or later, 12GB minimum, with 32GB **strongly** preferred (Ex: 32GB Volta)
  * 2 x Secondary / developer servers (GPU) - 8+ CPU cores, 64GB+ CPU RAM, 2-4 GPUs, 64GB+ disk, 1TB attached SSD
    * GPUs: Nvidia Pascal or later, 12GB minimum
  * 3 x Analyst stations (GPU) - 8+ CPU cores, 64GB+ CPU RAM, 1 TB attached SSD, 1-2 GPUs
    * GPUs: Nvidia Pascal or later, 12GB minimum, with 32GB **strongly** preferred (Ex: 32GB Volta)
  * For each, we can work together to setup Ubuntu with remote SSH admin, Nvidia drivers, & (Nvidia-enabled) Docker

* **Sponsors**: Near-term funding until the project finds a more sustainable path is welcome!

* **Subprojects**: We are focusing near-term on core data pipeline and simple analyses while building up to the discourse-graph-level ones

  * Orchestration tasks:
     * Python entity extractors: tweet -> text, URLs, bitcoin address, topics, ...
     * Python enrichment tasks: external APIs (factcheck, crypto, ...) and lightweight NLP algs (sentiment) and feed back to neo4j
     * Python data feed collectors: scripts that download feeds (factcheck, phishing, ...) and feed back to neo4j
  * Intervention campaigns: 
     * **Priority**: Untrialed drug misinformation - modeling, detection, analysis, report, & alert
     * Scams: Check URLs & blockchain addresses for known badness
     * Mapping bots & misinformers
  * Automation: Prototypes of
     
     * Community leader tools: Personalized alerting for community leaders to detect & respond to misinfo in their close social networks
  

## Contact

Please contact [Andrea Downing,  @ LightCollective] (https://www.linkedin.com/in/andreadowning/) for support and information

[Follow on Twitter: @BeLikeLight](https://twitter.com/BeLikeLight) 
