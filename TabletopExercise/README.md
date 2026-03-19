# Tabletop Exercise: Project "Broken Bridge"
**Scenario Focus:** 3rd Party API Failure & Supply Chain Disruption  
**Framework Alignment:** NIST SP 800-84 (Guide to Test, Training, and Exercise Programs)  
**Related Risk ID:** RS-1004 (3rd Party API Dependency)

---

## 1. Exercise Objective
To evaluate Aether Edge’s operational resilience and communication protocols during a critical failure of a primary payment processor. This exercise tests the coordination between the DevOps, Legal, and Customer Success teams.

## 2. The Narrative (The Incident)
* **09:00 AM:** Internal monitoring alerts show a 100% failure rate for the **AetherPay API**. 
* **09:15 AM:** Customer Support reports a surge in tickets (50+ in 15 minutes) regarding failed checkouts.
* **09:45 AM:** The vendor’s status page is unresponsive. No official communication has been received from their NOC.

## 3. Inject 1: The "Social Media" Factor (T+1 Hour)
> **Update:** A viral post on X (Twitter) claims Aether Edge has been "hacked" because payments are failing. 
* **Discussion Question:** Does our Incident Response Plan (IRP) include a "Public Communications" trigger? 
* **Decision Point:** Who is authorized to post a correction to social media to prevent reputational damage?

## 4. Inject 2: The "Contractual" Reality (T+3 Hours)
> **Update:** Legal reviews the vendor contract. The Service Level Agreement (SLA) excludes "acts of cyber-terrorism" or "upstream provider outages" from financial uptime guarantees.
* **Discussion Question:** If we lose $50k in transaction revenue today, do we have a secondary payment gateway ready for "Fail-over"?
* **Decision Point:** At what point do we activate our Business Continuity Plan (BCP) to switch providers?

## 5. Expected Outputs & Action Items
