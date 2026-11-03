# 🚀 Hybrid AI Framework: Product Strategy to Agile Execution

📌 **Live Dashboard:** [View this complete Case Study & Prompt Framework in Notion](https://plain-vulture-da9.notion.site/PROMPT-ENGINEERING-PROJECT-40d086dbe3b18061a7b6ed7aa294d984?source=copy_link)
## Executive Summary
This repository demonstrates a 4-stage system prompt architecture designed for Product and Project Managers. Instead of generating unconstrained raw text, this framework enforces structured methodology—moving sequentially from persona simulation to RICE prioritization, Product Requirements Document (PRD) creation, and Work Breakdown Structure (WBS) sprint tickets.

---

## 🛠 System Architecture

### Phase 1: Persona & Pain Point Simulator
* **Objective:** Synthesize qualitative user feedback and extract root-cause frustrations.
* **Prompt Engineering:**
#PROMPT 1:-

> **System Context:** You are an AI simulating the persona of three distinct e-commerce customers.
> 
> 
> **Task:** I am a Product Manager exploring a new "Smart One-Click Return" feature for our mobile app. I need to understand user pain points with the current manual return process.
> 
> **Instructions:**
> 
> 1. Generate three distinct user personas (Name, Age, Tech-Savviness, and Shopping Frequency).
> 2. Write a short, first-person narrative from each persona detailing their biggest frustration with returning items online.
> 3. Synthesize their feedback into a bulleted list of the top 3 core user pain points.
>
> Phase 2: RICE Prioritization Engine
Objective: Evaluate potential solution features against Reach, Impact, Confidence, and Effort metrics.

Prompt Engineering:
#PROMPT 2: The RICE Prioritization Engine**

> **System Context:** You are an AI simulating a Lead Product Manager.
> 
> 
> **Task:** Take the top 3 user pain points identified in the previous step regarding the manual return process and propose solutions.
> 
> **Instructions:**
> 
> 1. Propose 3 distinct technical features that would solve these specific pain points (e.g., QR code drop-offs, AI sizing feedback, instant refunds).
> 2. Evaluate each of the 3 features using the RICE prioritization framework (Reach, Impact, Confidence, Effort).
> 3. Present the RICE evaluation in a structured Markdown table.
> 4. State clearly which single feature should be prioritized for the MVP (Minimum Viable Product) based on the highest RICE score.
> 
>  5. **Prioritization Rationale:** Add a 2-sentence breakdown explaining the explicit trade-off rationale—why the winning MVP feature outranked the runner-up in terms of Effort vs. Impact.

Phase 3: Automated PRD Generator
Objective: Transform the prioritized feature into a structured, board-ready Product Requirements Document.

Prompt Engineering:

#PROMPT 3: The PRD Generator**

> **System Context:** You are an AI simulating a Senior Product Manager.
> 
> 
> **Task:** Take the winning MVP feature identified in the RICE prioritization step and draft a concise, board-ready Product Requirements Document (PRD).
> 
> **Instructions:**
> Format the PRD using Markdown with the following strict sections:
> 
> 1. **Executive Summary:** A two-sentence overview of the feature and its goal.
> 2. **Target Audience:** Who this feature is for (referencing the previous personas).
> 3. **User Stories:** Write 3 standard agile user stories (Format: "As a [type of user], I want [an action] so that [a benefit/value]").
> 4. **Success Metrics (KPIs):** List 2 measurable metrics to determine if the launch is successful.
> 5. **Out of Scope:** List 1 related feature that will explicitly NOT be built in this MVP phase to prevent scope creep.


Phase 4: Agile Execution & Risk Register
Objective: Translate product strategy directly into actionable 4-week sprint tickets and risk mitigation plans.

Prompt Engineering:

#PROMPT 4: The Project Execution Breakdown**

> **System Context:** You are an AI simulating a Technical Project Manager.
> 
> 
> **Task:** Translate the PRD generated in the previous step into an actionable execution plan for the engineering and design teams.
> 
> **Instructions:**
> 
> 1. **Work Breakdown Structure (WBS):** Break the feature down into 3 core phases (e.g., Design, Backend, Frontend).
> 2. **Sprint Timeline:** Create a high-level 4-week Gantt-style timeline in a Markdown table.
> 3. **Actionable Tickets:** Draft the first 3 Jira/Kanban tickets required to start the work (Include Ticket Title, Assignee Role, and Acceptance Criteria).
> 4. **Risk Register:** Identify the top 2 execution risks for this project and provide a one-sentence mitigation strategy for each.
> 5. **Risk Assessment Logic:** Provide a brief rationale for why Risk #1 was identified as the highest severity threat to the sprint launch.


#Complete Execution Case Study=

### 1. Generated Personas & Pain Points
<u>**PROMPT**</u>  1:- 

**The Persona & Pain Point Simulator**

> **System Context:** You are an AI simulating the persona of three distinct e-commerce customers.
> 
> 
> **Task:** I am a Product Manager exploring a new "Smart One-Click Return" feature for our mobile app. I need to understand user pain points with the current manual return process.
> 
> **Instructions:**
> 
> 1. Generate three distinct user personas (Name, Age, Tech-Savviness, and Shopping Frequency).
> 2. Write a short, first-person narrative from each persona detailing their biggest frustration with returning items online.
> 3. Synthesize their feedback into a bulleted list of the top 3 core user pain points.
Persona 1: The Hesitant Adopter

Name: Barbara

Age: 62

Tech-Savviness: Low

Shopping Frequency: Occasional (1-2 times a month)

Narrative:
"I get so flustered when something I order doesn’t fit. The app usually tells me I need to print a return label, but I haven't owned a printer in years. I end up having to call customer service or ask my daughter to help me get a QR code on my phone. Then, I have to find a specific shipping store, remember to bring the original box, and hope I taped it up right. It’s such a headache that sometimes I just keep clothes I don't even want."

Persona 2: The Efficiency Optimizer

Name: Marcus

Age: 34

Tech-Savviness: High

Shopping Frequency: Very Frequent (Multiple times a week)

Narrative:
"I buy everything from groceries to electronics on my phone, so returns are just a cost of doing business. My biggest frustration is the digital friction. To return one cable, I have to dig through my order history, click through five screens answering 'Why are you returning this?', bypass multiple prompts trying to offer me store credit, and finally generate a barcode. I don't have ten minutes to waste managing a $20 return. I just want to tap a button, drop the item naked at a kiosk, and get back to my day."

Persona 3: The Wardrober

Name: Chloe

Age: 23

Tech-Savviness: Moderate to High

Shopping Frequency: Frequent (Weekly)

Narrative:
"I always order two sizes of everything to try on at home, so returning half my cart is literally part of my shopping routine. What drives me crazy is the lack of trust and the delayed refunds. The app makes me upload photos of the tags just to get the return approved, which feels insulting. Then, after I finally drop it off, my money is tied up in a black hole for two weeks while it ships back to the warehouse. I need that money back in my account faster so I can buy other things."

Top 3 Core User Pain Points

High Digital Friction: Users are frustrated by multi-step authorization processes, buried order histories, mandatory questionnaires, and forced photo uploads just to initiate a return.

Physical Logistics & Handoff: The physical requirements of returning an item—sourcing a printer for labels, repackaging the item securely, and locating specific carrier drop-off points—create a significant barrier, especially for less tech-savvy or time-poor users.

Refund Anxiety & Capital Tie-Up: Users lack visibility once an item is dropped off and resent waiting weeks for warehouse processing. The delay in returning funds restricts their purchasing power and reduces trust in the brand.



---

### 2. RICE Evaluation & MVP Selection
**Proposed Technical Features**

* **Smart-Auth One-Click Initiation:** Solves high digital friction by utilizing an internal algorithmic trust score to instantly approve returns for accounts in good standing, bypassing all mandatory questionnaires and photo uploads.
* **Box-Free QR Code Drop-Offs:** Solves physical logistics by integrating with carrier APIs to generate a dynamic barcode, allowing users to hand over unboxed, unlabelled items directly to a local retail kiosk.
* **Instant Scan-to-Refunds:** Solves refund anxiety and capital tie-up by triggering the refund to the user's payment method the exact moment the shipping carrier scans the package at drop-off, rather than waiting for warehouse receipt.

**RICE Prioritization Evaluation**

*(Assuming a baseline Reach of 10,000 return transactions per month. Impact: 3=Massive, 2=High. Confidence: 1.0=100%, 0.8=80%. Effort = Person-months).*

| Feature | Reach | Impact | Confidence | Effort | RICE Score |
| --- | --- | --- | --- | --- | --- |
| **Smart-Auth One-Click Initiation** | 10,000 | 2 | 100% (1.0) | 1 | **20,000** |
| **Instant Scan-to-Refunds** | 10,000 | 3 | 70% (0.7) | 3 | **7,000** |
| **Box-Free QR Code Drop-Offs** | 10,000 | 3 | 80% (0.8) | 4 | **6,000** |

**MVP Prioritization Decision**

The **Smart-Auth One-Click Initiation** must be prioritized as the Minimum Viable Product (MVP).

**Prioritization Rationale**

While the Instant Scan-to-Refund runner-up delivers a slightly higher overall impact on customer satisfaction, it requires complex third-party payment gateway integration and introduces a high fraud risk that drives up our engineering Effort and lowers our Confidence. Smart-Auth One-Click Initiation decisively wins the MVP slot because it utilizes internal logic we already control to strip away UX friction for a fraction of the development cost, yielding a massive, immediate return on investment.

---

### 3. Product Requirements Document (PRD)
**1. Executive Summary**
The Smart-Auth One-Click Initiation feature eliminates digital friction in the returns process by utilizing an internal algorithmic trust score to instantly approve returns for customers in good standing. By bypassing mandatory questionnaires and photo uploads, this MVP aims to significantly reduce the time and effort required for users to initiate a return, thereby driving higher customer satisfaction and lifetime value.

**2. Target Audience**
This feature is designed primarily for high-frequency shoppers like the "Efficiency Optimizer" (Marcus) who have zero tolerance for digital friction, as well as the "Wardrober" (Chloe) who relies on seamless returns as a core part of their regular purchasing cycle.

**3. User Stories**

* As an Efficiency Optimizer, I want to initiate a return with a single tap so that I can manage my order without wasting time navigating mandatory feedback forms.
* As a Wardrober, I want my return approved instantly without being forced to upload photos of product tags so that I feel trusted by the brand and can complete my shopping routine seamlessly.
* As a Customer Support Administrator, I want the system to automatically authorize returns for high-trust users so that I can focus my manual review efforts exclusively on high-risk or flagged accounts.

**4. Success Metrics (KPIs)**

* **Time-to-Initiate:** A 50% reduction in the average time it takes a user to complete the return request flow (measured from the moment they click "Return Item" to receiving the final return confirmation screen).
* **Return Initiation Drop-off Rate:** A 30% decrease in the number of users who abandon the return process midway through the digital authorization flow.

**5. Out of Scope**

* **Instant Scan-to-Refunds:** Triggering immediate financial refunds to the user's payment gateway upon the shipping carrier's barcode scan is explicitly excluded from this MVP to avoid complex third-party payment integrations and mitigate uncalculated fraud risks during the initial rollout.

---

### 4. Agile Execution & Risk Mitigation Plan
**1. Work Breakdown Structure (WBS)**

* **Phase 1: Design & Architecture**
* Map out the updated user journey to eliminate the legacy questionnaire and photo upload screens.
* Design the new "One-Click Return" UI state and the instant authorization success screen.
* Define backend data schemas for the internal algorithmic trust score and API request/response payloads.


* **Phase 2: Backend & Trust Algorithm Development**
* Develop the internal trust-scoring logic based on existing user data (e.g., account age, return rate, past fraud flags).
* Build the new `POST /returns/initiate-smart-auth` endpoint to process the one-click request.
* Implement fallback logic to route low-trust users to the manual review queue automatically.


* **Phase 3: Frontend Integration & Quality Assurance**
* Strip out legacy frontend dependencies tied to the mandatory questionnaire.
* Wire the new UI components to the smart-auth API endpoint.
* Conduct end-to-end (E2E) testing across user states (high-trust vs. low-trust) and deploy to staging.



**2. Sprint Timeline**

| Task Category | Week 1 | Week 2 | Week 3 | Week 4 |
| --- | --- | --- | --- | --- |
| **UX/UI Design & Prototyping** | █ █ █ |  |  |  |
| **Backend API & Schema Architecture** | █ █ █ |  |  |  |
| **Trust Score Algorithm Development** |  | █ █ █ |  |  |
| **Frontend UI Implementation** |  | █ █ █ | █ █ █ |  |
| **API & Frontend Integration** |  |  | █ █ █ |  |
| **E2E Testing & Bug Triage** |  |  |  | █ █ █ |
| **Staging Deployment & Launch Prep** |  |  |  | █ █ █ |

**3. Actionable Tickets**

* **Ticket 1: Define & Implement Trust Score Evaluation Logic**
* **Assignee Role:** Backend Engineer
* **Acceptance Criteria:** A backend function is created that accepts a `UserID` and returns a boolean (`isTrusted`). The logic must evaluate the user's account age (>30 days) and historical return rate (<40% over 6 months). If criteria are met, the function returns `true`; otherwise, it returns `false`.


* **Ticket 2: Overhaul Return Initiation UI (Figma)**
* **Assignee Role:** UX/UI Designer
* **Acceptance Criteria:** Figma prototypes are delivered showing the removal of the multi-step questionnaire. The design must include a clear "Return Item" confirmation button, a loading state, and an "Instant Approval" success modal with next steps for drop-off.


* **Ticket 3: Decouple Legacy Frontend Form Dependencies**
* **Assignee Role:** Frontend Engineer
* **Acceptance Criteria:** The existing mobile app return flow is modified to conditionally bypass the questionnaire screens. Bypassing these screens must not trigger null-reference crashes when the final return payload is submitted to the backend.



**4. Risk Register**

* **Risk 1: False Negatives in Trust Scoring:** The algorithm may be too strict, accidentally flagging high-value, high-frequency shoppers (like our "Wardrober" persona) as low-trust and forcing them into the manual review process.
* **Mitigation Strategy:** Run the trust algorithm in a silent "shadow mode" against historical database records for three days prior to launch to calibrate the threshold and ensure false negatives are kept under 2%.


* **Risk 2: Legacy Payload Failures:** Bypassing the mandatory questionnaire might cause backend database insertions to fail if the legacy system requires non-null values for the "Reason for Return" fields.
* **Mitigation Strategy:** Hardcode a default "Smart-Auth Automated Return" string into the payload for bypassed fields to satisfy existing database constraints without requiring a structural database migration.



**5. Risk Assessment Logic**
False negatives in trust scoring were identified as the highest severity threat because they directly undermine the core objective of the MVP. If the algorithm fails to instantly approve our most loyal, high-frequency customers, we actively degrade their user experience and violate the brand trust we are attempting to build, potentially causing high-value customer churn before engineering can deploy a patch.

