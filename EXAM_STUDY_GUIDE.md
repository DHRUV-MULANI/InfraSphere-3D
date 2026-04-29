# HS 225002 - Infrastructure Planning & Management
# CONNECTED STUDY GUIDE (60 Marks Total)

---

## THE BIG PICTURE: How Everything Connects

```
EVERY infrastructure project follows this chain:

  VIABILITY CHECK ──> RISK ASSESSMENT ──> ASSET MANAGEMENT ──> SMART MONITORING
  (Should we build?)   (What can go wrong?)  (How to maintain?)    (How to optimize?)
       │                     │                     │                      │
    NPV, IRR, BCR       Risk Matrix          Lifecycle Planning      IoT, Digital Twin
    PPP Model choice     EMV calculation      Condition Assessment    BIM, Sensors
    Feasibility Study    Risk Allocation      Valuation Methods       Data Analytics
```

**This is the ONE mental model. Every case study is just this chain applied to a real project.**

---

## PART A: THEORY (20 Marks) - The 4 Pillars

---

### PILLAR 1: PROJECT VIABILITY ("Should we build it?")

**Core Question:** Will this project give returns > costs?

**Decision Tools:**
| Tool | Formula | Decision Rule |
|------|---------|---------------|
| **NPV** | Sum of [CF_t / (1+r)^t] - Initial Investment | NPV > 0 = Accept |
| **IRR** | Rate where NPV = 0 (trial & error) | IRR > required rate = Accept |
| **BCR** | PV of Benefits / PV of Costs | BCR > 1 = Accept |
| **Payback** | Initial Investment / Annual Cash Flow | Shorter = Better |

**Two types of viability:**
- **Financial Viability** = Will investors get returns? (private perspective)
- **Economic Viability** = Will society benefit? (includes externalities, social benefits)

**When private returns are low but social returns are high → Government steps in via PPP**

**PPP Models (memorize this spectrum):**
```
MORE Government Control ◄──────────────────────► MORE Private Control

Service    Management   Lease    BOT    BOOT    DBFO    BOO    Privatization
Contract   Contract                                    
                                 │       │       │      │
                              Dabhol  Vizhinjam Airport  
                              (power)  (port)  (Delhi/Mum)
```

| Model | Build | Own | Operate | Transfer | Finance |
|-------|-------|-----|---------|----------|---------|
| BOT | Private | Govt | Private | Yes | Private |
| BOOT | Private | Private→Govt | Private | Yes | Private |
| DBFO | Private | Govt | Private | Yes | Private |
| BOO | Private | Private | Private | No | Private |

**Feasibility Study = Technical + Financial + Economic + Environmental + Social**

---

### PILLAR 2: RISK MANAGEMENT ("What can go wrong?")

**Process:** Identify → Assess → Mitigate → Monitor (cycle repeats)

**Risk Matrix = Probability x Impact**

```
              IMPACT
         Low    Med    High
  High │  M   │  H   │  VH  │
Prob Med │  L   │  M   │  H   │
  Low │  VL  │  L   │  M   │
```

**Risk Types in Infrastructure (remember with: PFCEO)**
- **P**olitical - govt change, policy reversal (Dabhol: BJP cancelled project)
- **F**inancial - cost overrun, currency, interest rate (Dabhol: dollar tariff in rupee economy)
- **C**onstruction - delays, technical issues
- **E**nvironmental - pollution, clearances, natural disasters
- **O**perational - demand risk, maintenance, performance (Airtel: Jio disruption)

**Risk Response Strategies (ATMA):**
- **A**void - eliminate the threat entirely (don't do the project)
- **T**ransfer - shift to someone else (insurance, contracts, guarantees)
- **M**itigate - reduce probability or impact (better design, monitoring)
- **A**ccept - live with it (low probability, low impact risks)

**Risk Allocation in PPP = Give each risk to the party best able to manage it**
- Construction risk → Private (they build)
- Demand/revenue risk → Shared (both influence it)
- Political/regulatory risk → Government (they control policy)
- Force majeure → Shared

**EMV (Expected Monetary Value) = Probability x Impact (in Rs.)**
- Used to prioritize which risks need most attention
- Higher EMV = more critical risk

**Monte Carlo Simulation** = Run thousands of random scenarios → get probability distribution of outcomes (NPV, cost, time). Shows range of possible results, not just one number.

**Sensitivity Analysis** = Change one variable at a time → see how much the output (NPV) changes. Identifies which variables matter most.

---

### PILLAR 3: ASSET MANAGEMENT ("How to maintain what we built?")

**Asset = anything of value to the organization (roads, bridges, pipelines, networks)**

**ISO 55000** = International standard for asset management
- Align assets with organizational objectives
- Lifecycle approach (not just maintenance)
- Balance cost, risk, and performance

**Asset Lifecycle:**
```
Plan → Acquire/Create → Operate → Maintain → Renew/Dispose
  │                                              │
  └──────────── feeds back to ◄──────────────────┘
```

**Valuation Methods:**
| Method | What it means | When to use |
|--------|--------------|-------------|
| Historical Cost | What you paid originally | Accounting/books |
| Replacement Cost | What it would cost to replace today | Insurance |
| Market Value | What someone would pay for it | Selling |
| Depreciated Replacement Cost | Replacement cost minus wear & tear | Fair value of used asset |

**Maintenance Strategies (from dumb to smart):**
```
Reactive ──> Preventive ──> Condition-Based ──> Predictive
(fix when    (scheduled     (monitor & fix     (AI predicts
 broken)      intervals)     when needed)        failure)
   │              │               │                  │
 Cheapest      Medium cost     Needs sensors     Needs IoT/AI
 Most risky    Some waste      Efficient         Most efficient
```

**Condition Assessment** = Rating asset health (1-5 scale typically)
- Drives maintenance priority
- Feeds into capital planning

**Asset Management Plan** = Document covering:
- Asset inventory (what do we have?)
- Condition assessment (what state is it in?)
- Lifecycle strategy (maintain/renew/dispose?)
- Financial plan (how much money needed?)
- Risk assessment (what if it fails?)

---

### PILLAR 4: SMART INFRASTRUCTURE ("Technology overlay on everything")

**Smart Infrastructure = Traditional Infrastructure + Digital Technology**

**Key Technologies:**
| Tech | What it does | Example |
|------|-------------|---------|
| **IoT** | Sensors collecting real-time data | Traffic sensors, water quality monitors |
| **Digital Twin** | Virtual replica of physical asset | Simulate bridge stress without testing real bridge |
| **BIM** | 3D model for design + construction | Clash detection before building |
| **AI/ML** | Pattern recognition, prediction | Predictive maintenance, demand forecasting |
| **Big Data Analytics** | Process massive datasets | City-wide traffic optimization |

**Smart City Domains:**
- Smart Transport (GPS tracking, adaptive signals, EV charging)
- Smart Grid (smart meters, renewable integration, demand response)
- Smart Water (leak detection, quality monitoring, automated treatment)
- Smart Buildings (energy management, automated HVAC)

**Cybersecurity** = Critical because smart infra is connected → vulnerable to attacks
- SCADA systems for critical infrastructure
- Data privacy concerns
- Need defense-in-depth approach

**How Smart connects to other pillars:**
```
Smart Infra → better Asset Management (predictive maintenance via sensors)
Smart Infra → better Risk Management (real-time monitoring, early warning)
Smart Infra → better Project Viability (data-driven decisions, efficiency gains)
```

---

## PART B: CASE STUDIES (20 Marks) - Theory Applied

---

### CASE STUDY MAP: Which theory applies where?

```
CASE STUDY              MAIN THEORY TOPICS
─────────────────────────────────────────────────
Dabhol Power         →  Project Viability + Risk Management
                        (PPP failure, political risk, financial risk)

Airport Priv.        →  Project Viability + Risk Management  
(Delhi/Mumbai)          (PPP success, bidding process, JVC model)

Vizhinjam Port       →  Project Viability + Risk Management
                        (PPP, viability gap funding, DBFOT model)

Airtel/Jio           →  Asset Management + Smart Infrastructure
                        (telecom infra, disruption, network assets)

Indian Railways      →  Asset Management + Project Viability
(Gandhidham)            (rail infra, port connectivity, BOT)

AirAsia India        →  Project Viability + Risk Management
                        (market entry, JV structure, regulatory risk)
```

---

### CASE 1: DABHOL POWER PROJECT (The Classic PPP Failure)

**What:** $3 billion, 2184 MW gas power plant by Enron in Maharashtra
**PPP Model:** Effectively BOO (Build-Own-Operate)
**Sole Customer:** MSEB (Maharashtra State Electricity Board)

**What went wrong (connect to Risk theory):**
| Risk Type | What Happened |
|-----------|--------------|
| Political | BJP-Shiv Sena govt cancelled project in 1995 (Munde Committee) |
| Financial | Dollar-denominated tariff in rupee economy → MSEB couldn't pay |
| Demand | Over-sized for state's ability to absorb power |
| Regulatory | No competitive bidding, fast-tracked approvals |
| Contractual | One-sided PPA favoring Enron (World Bank warned!) |

**Key Lessons for exam:**
- Risk allocation was wrong → most risk on government/MSEB
- No competitive bidding → inflated costs
- World Bank warned project was too large and expensive → ignored
- Political risk not mitigated → no multi-party consensus
- Viability was questionable from start → LNG too expensive as fuel
- Credit support: GoM guarantee + GoI counter-guarantee + escrow → still failed

**If asked "what should have been done differently":**
1. Competitive bidding (transparent process)
2. Smaller project size matched to demand
3. Risk sharing (not all on MSEB)
4. Rupee-denominated tariff
5. Multi-party political consensus before starting
6. Heed World Bank assessment

---

### CASE 2: AIRPORT PRIVATIZATION (Delhi & Mumbai) (PPP Done Better)

**What:** Rs.54 billion modernization of Delhi & Mumbai airports
**PPP Model:** JVC (Joint Venture Company) - 74% Private + 26% AAI
**Agreement:** OMDA (Operations, Management & Development Agreement) - 30+30 years

**Key Structure:**
- Revenue sharing model (% of gross revenue to govt)
- Highest revenue share bid = winner
- 4-phase evaluation: Mandatory → Financial Commitment → Technical PreQual (80% cutoff) → Financial Bid

**What went right vs Dabhol:**
| Aspect | Dabhol (Failed) | Airport (Worked) |
|--------|----------------|-----------------|
| Bidding | No competition | 9 pre-qualified bidders |
| Transparency | Opaque | Multiple review committees (EC, GRC, GETE, CoS, IMG, EGoM) |
| Risk sharing | All on govt | Shared (revenue sharing model) |
| Political | No consensus | EGoM with multi-party ministers |
| Regulation | None | AERA (Airport Economic Regulatory Authority) |

**Controversy:** GETE (headed by E. Sreedharan) qualified only GMR-Fraport, downgraded Reliance-ASA → raised bias concerns. But process had multiple checks.

---

### CASE 3: VIZHINJAM PORT (PPP with Viability Gap)

**What:** Deep-water container transshipment port in Kerala
**PPP Model:** DBFOT (Design, Build, Finance, Operate, Transfer)
**Key Player:** Adani Ports (concessionaire), GoK (Government of Kerala)

**Why this case matters:**
- Project is NOT financially viable without government support
- Returns too low for private investors to finance civil works alone
- IFC recommended "Modified Landlord Model"
- **Viability Gap Funding** = Government pays for breakwater, dredging, road/rail links
- Private sector builds and operates terminal (superstructure)

**Connect to theory:**
- NPV likely negative without govt grant → needs viability gap funding
- High risk: transshipment traffic unpredictable, competition from Colombo
- Multiple failed bid attempts (2007, 2008-09, 2010-12) before Adani won
- Asset life (50-100 years) >> Concession period (25-40 years) → depreciation mismatch

---

### CASE 4: AIRTEL (Telecom Infrastructure Disruption)

**What:** Airtel facing market disruption from Reliance Jio's entry (Sept 2016)
**Core Issue:** Voice revenue collapsing → must transition to data

**Key Numbers:**
- Jio: 100 million customers in 170 days, free voice, Rs.50/GB data
- Airtel ARPU crashed: Rs.200 → Rs.145
- Industry debt: Rs.4.6 lakh crore
- Revenue decline: 18.1% YoY (2017)

**Connect to Asset Management:**
- Telecom network = massive infrastructure asset (towers, spectrum, fiber)
- Airtel's asset strategy: "minutes factory" → lowest cost per minute
- Need to repurpose 2G/3G assets for 4G data
- Spectrum = expensive asset (Jio paid Rs.12,847 crore for BWA spectrum alone)

**Connect to Smart Infrastructure:**
- VoLTE technology (Voice over LTE) - Jio was first
- Data-centric network vs voice-centric
- 4G infrastructure enabling IoT, smart services

---

### CASE 5: INDIAN RAILWAYS - GANDHIDHAM (Asset Planning)

**What:** Railway infrastructure serving Kandla & Mundra ports in Gujarat
**Focus:** Capacity planning, asset utilization, port-rail connectivity

**Connect to Asset Management:**
- Rail network as long-life infrastructure asset
- Gauge conversion (MG to BG) as asset renewal
- Capacity constraints → need expansion planning
- BOT model for container berths at Kandla port

**Connect to Project Viability:**
- Mundra Port = JV between Gujarat Govt & Adani (GAPL) - private port model
- Kandla = Government-owned major port
- Traffic projections drive investment decisions
- Competition between road and rail for hinterland cargo

---

### CASE 6: AIRASIA INDIA (Market Entry & Regulatory Risk)

**What:** AirAsia (Malaysia) entering India through JV with Tata Sons (2013)
**PPP angle:** FDI in aviation, regulatory framework

**Key Risks (connect to Risk theory):**
| Risk | Detail |
|------|--------|
| Regulatory | FIPB approval, DGCA clearance, Supreme Court challenge |
| Political | Subramanian Swamy petition, election commission approach |
| Financial | Continuous losses (Rs.940M in 2014, Rs.1820M in 2015-16) |
| Internal | Shareholder conflict (Bhatia accused Fernandes of remote control) |
| Market | Competition from IndiGo, SpiceJet, Jet Airways |

**Key Strategy (Low Cost Carrier model):**
- Single aircraft type (A320-200) → low maintenance cost
- Point-to-point routes → no hub dependency
- No frills → no free food, charge for extras
- 25-min turnaround → high aircraft utilization
- Online booking → lower distribution cost

---

## PART C: NUMERICAL/SUMS (20 Marks) - Formulas & Methods

---

### FORMULA SHEET

#### 1. NPV (Net Present Value)
```
NPV = -Initial Investment + CF1/(1+r)^1 + CF2/(1+r)^2 + ... + CFn/(1+r)^n

Example: Investment = 10,000, Cash flows = 3,000/yr for 5 years, r = 10%
NPV = -10,000 + 3000/1.1 + 3000/1.21 + 3000/1.331 + 3000/1.4641 + 3000/1.6105
    = -10,000 + 2727 + 2479 + 2254 + 2050 + 1863
    = 1,373 → ACCEPT (positive)
```

#### 2. IRR (Internal Rate of Return)
```
Find rate 'r' where NPV = 0
Method: Try two rates, interpolate

IRR = r1 + [NPV1 / (NPV1 - NPV2)] x (r2 - r1)

where NPV1 is positive (at r1) and NPV2 is negative (at r2)

Example: NPV at 15% = +500, NPV at 20% = -200
IRR = 15% + [500/(500+200)] x (20%-15%) = 15% + 3.57% = 18.57%
```

#### 3. BCR (Benefit-Cost Ratio)
```
BCR = PV of Benefits / PV of Costs

Example: PV Benefits = 15,000, PV Costs = 12,000
BCR = 15,000/12,000 = 1.25 → ACCEPT (> 1)
```

#### 4. Payback Period
```
Simple: Payback = Initial Investment / Annual Cash Flow
Example: Investment = 10,000, Annual CF = 2,500
Payback = 10,000/2,500 = 4 years

If unequal cash flows: cumulate until investment is recovered
Year 1: 2000 (cumulative: 2000)
Year 2: 3000 (cumulative: 5000)
Year 3: 4000 (cumulative: 9000)
Year 4: 3000 (cumulative: 12000) ← recovered 10,000 somewhere in Year 4
Payback = 3 + (10000-9000)/3000 = 3.33 years
```

#### 5. EMV (Expected Monetary Value) for Risk
```
EMV = Probability x Impact (monetary)

Example: 
Risk A: 30% chance of Rs.10 lakh loss → EMV = 0.3 x 10 = Rs.3 lakh
Risk B: 10% chance of Rs.50 lakh loss → EMV = 0.1 x 50 = Rs.5 lakh
→ Risk B is more critical despite lower probability
```

#### 6. Risk Priority Number
```
Risk Score = Likelihood (1-5) x Consequence (1-5)

Score 1-4: Low priority
Score 5-9: Medium priority  
Score 10-15: High priority
Score 16-25: Critical → immediate action
```

#### 7. Depreciation (for Asset Valuation)
```
Straight Line: Depreciation/year = (Cost - Salvage Value) / Useful Life

Example: Asset cost = 50,000, Salvage = 5,000, Life = 10 years
Annual Depreciation = (50,000 - 5,000)/10 = Rs.4,500/year
Book Value after 6 years = 50,000 - (4,500 x 6) = Rs.23,000

Depreciated Replacement Cost = Replacement Cost x (Remaining Life / Total Life)
Example: Replacement Cost = 80,000, Used 6 of 10 years
DRC = 80,000 x (4/10) = Rs.32,000
```

#### 8. Present Value (basic building block)
```
PV = FV / (1+r)^n

Example: Rs.10,000 received after 3 years, r = 8%
PV = 10,000 / (1.08)^3 = 10,000 / 1.2597 = Rs.7,938
```

#### 9. Annuity Factor (for equal annual cash flows)
```
PV of Annuity = Annual CF x [(1 - (1+r)^-n) / r]

Example: Rs.5,000/year for 5 years at 10%
= 5,000 x [(1 - 1.1^-5) / 0.1]
= 5,000 x [(1 - 0.6209) / 0.1]
= 5,000 x 3.791
= Rs.18,955
```

---

### QUICK COMPARISON: When to use which tool?

| Question | Use This |
|----------|---------|
| "Is project worth doing?" | NPV (best overall) |
| "What rate of return?" | IRR |
| "Benefits vs costs for society?" | BCR (used in govt projects) |
| "How fast do I get money back?" | Payback Period |
| "Which risk is most critical?" | EMV or Risk Matrix |
| "What's the asset worth now?" | Depreciated Replacement Cost |
| "Range of possible outcomes?" | Monte Carlo Simulation |
| "Which variable matters most?" | Sensitivity Analysis |

---

## QUICK REVISION: Connect the Dots

### How to answer ANY case study question:

1. **Identify the PPP model** used (BOT/BOOT/DBFO/BOO/JVC)
2. **Check viability**: Was NPV analysis done? Financial vs economic viability?
3. **List risks**: Use PFCEO framework (Political, Financial, Construction, Environmental, Operational)
4. **Evaluate risk allocation**: Who bears what risk? Is it allocated to the right party?
5. **Asset management angle**: What assets are involved? Lifecycle stage? Maintenance strategy?
6. **Smart infra angle**: Could technology have helped? How?
7. **What went wrong/right**: Connect to theory concepts

### One-line case study summaries:

| Case | One Line | Key Theory |
|------|----------|-----------|
| **Dabhol** | PPP gone wrong - political risk + one-sided contracts + no competition | Risk misallocation, viability ignored |
| **Airport** | PPP done right - transparent bidding + revenue sharing + multiple oversight | Good risk allocation, competitive process |
| **Vizhinjam** | Needs govt money to work - viability gap funding essential | Financial vs economic viability |
| **Airtel** | Infra disruption - voice assets becoming data assets | Asset lifecycle, smart transition |
| **Railways** | Capacity planning for growing ports | Asset management, demand forecasting |
| **AirAsia** | Foreign entry risks - regulatory + JV conflicts | Political & regulatory risk |

---

## EXAM STRATEGY

**Theory (20 marks):** Write definitions briefly, then USE DIAGRAMS. Draw the risk matrix, the asset lifecycle, the PPP spectrum. Examiners love visual answers.

**Case Study (20 marks):** Start with 2-line context of the case → identify which theory applies → apply theory framework → give specific examples from the case → conclude with lessons learned.

**Numerical (20 marks):** Show ALL steps. Write the formula first. Substitute values. Calculate step by step. State the decision rule. Give conclusion. Even if your arithmetic is slightly off, the method marks come from showing the process.

---

*Good luck tomorrow!*
