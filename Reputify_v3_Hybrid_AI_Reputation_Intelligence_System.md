# 🚀 **Reputify v3 – AI Reputation Intelligence & Engagement System**

**Version:** 3.0 (De-risked & Scalable)  
**Purpose:** Build a multilingual, AI-powered SaaS platform for managing, analyzing, and improving business reputation — safely and affordably.  
**Focus:** Real-time insights, smart analytics, and human-centered AI engagement using a **hybrid data collection model** combining both **official APIs** and **third-party automation platforms** (Apify) for comprehensive coverage.

---

## 1. **The Problem: Digital Reputation Blind Spots**

Small and medium businesses often face the same critical challenge — **they don’t know what customers are saying about them until it’s too late.**

### **Common Problems:**

- ⏰ **Time Constraints:** Owners can’t monitor reviews across platforms daily.
- ⚠️ **Unnoticed Negative Feedback:** Damaging comments go unanswered.
- 🧩 **Scattered Data:** Google and Facebook reviews aren’t connected.
- 🔍 **Lack of Insights:** No clear way to know _why_ ratings drop.
- 🔕 **Reactive Management:** Issues are discovered only after customers leave.

### **Business Impact:**

- 💔 Loss of trust, customers, and revenue due to unmanaged online perception.

---

## 2. **The Reputify Solution**

> **Reputify** helps businesses actively monitor, understand, and improve their online reputation through multilingual AI using a **hybrid data collection approach** that combines official APIs with compliant automation platforms.

### **Core Value Proposition:**

**🔍 Listen → 🧠 Analyze → 🤖 Engage → 📈 Improve**

- **👂 Listen:** Gather all reviews and mentions across **7 key platforms** (Google Business, Facebook, Instagram, LinkedIn, YouTube, Reddit, TikTok) using **official APIs** and **cost-optimized automation** through a hybrid data collection model.
- **📊 Analyze:** Use NLP & ML to find patterns, emotions, and trends across all collected data with platform-specific insights.
- **💬 Engage:** Suggest human-approved AI responses in local languages with platform-appropriate tone and formatting.
- **🚀 Improve:** Predict rating trends and highlight issues to prevent crises across all monitored platforms.

---

## 3. **Evolution Overview**

| **Version**           | **Focus**                 | **Description**                                                                    |
| --------------------- | ------------------------- | ---------------------------------------------------------------------------------- |
| **v1 – Foundation**   | Review Management         | Centralized review platform with alerts & replies                                  |
| **v2 – Intelligence** | Smart Analytics           | Aspect-based insights, review plausibility analysis, predictive analysis           |
| **v3 – Engagement**   | Social Awareness & Ethics | Intent detection, AI engagement (human-approved), issue extraction, feedback loops |

🛡️ **Enhanced Data Collection:** _Implemented hybrid approach using official APIs + Apify automation for public social content_ (replaced high-risk direct scraping).

✅ **Total Features Now:** **14 Safe, Scalable, and Realistic Modules**

---

## 3.1 **Confirmed Platform Coverage (7 Platforms)**

| Platform      | What We Monitor                    | Access Method              | Cost Impact   | Risk Level |
| ------------- | ---------------------------------- | -------------------------- | ------------- | ---------- |
| **Google**    | Reviews on Google Business         | ✅ **Official Places API** | 💰 **Free**   | None       |
| **Facebook**  | Own page + public posts/hashtags   | ✅ **Graph API + Apify**   | 💰 **Hybrid** | Low        |
| **Instagram** | Comments, tags, hashtags           | ✅ **Graph API + Apify**   | 💰 **Hybrid** | Low        |
| **LinkedIn**  | Public hashtags & company mentions | ⚙️ **Apify Scrapers Only** | 💸 **Paid**   | Medium     |
| **TikTok**    | Hashtags, mentions in captions     | ⚙️ **Apify Scrapers**      | 💸 **Paid**   | Low        |
| **YouTube**   | Video comments & community posts   | ✅ **YouTube Data API**    | 💰 **Free**   | None       |
| **Reddit**    | Posts/comments mentioning brand    | ✅ **Reddit API**          | 💰 **Free**   | None       |

**Hybrid Data Collection Strategy:**

- **Official APIs (Primary):** Facebook/Instagram Graph APIs, Google Places, YouTube Data, Reddit API - all free within quotas
- **Apify Automation (Secondary):** TikTok scrapers, LinkedIn public content, Facebook/Instagram public mentions where APIs are limited
- **Cost Optimization:** 60-70% of data collected via free APIs, reducing overall operational costs
- **Result:** Comprehensive 7-platform coverage at ~$30-40/month operational cost

---

## 4. **System Overview**

### 🛠️ Tech Stack (Recommended)

| Layer                           | Technology                                                     | Purpose                                              |
| ------------------------------- | -------------------------------------------------------------- | ---------------------------------------------------- |
| **Frontend**                    | **Next.js (React + TypeScript)**                               | Dashboard & marketing website (SSR + SPA)            |
| **Styling**                     | **Tailwind CSS**                                               | Responsive UI and dark theme                         |
| **Backend**                     | **FastAPI (Python)**                                           | Core API server, data processing, JWT authentication |
| **Database**                    | **MongoDB Atlas**                                              | Stores businesses, mentions, AI data, alerts         |
| **Authentication**              | **JWT + bcrypt**                                               | Secure login and role-based access                   |
| **AI / NLP**                    | **OpenAI API + Hugging Face models**                           | Sentiment, intent, AI reply suggestions              |
| **Scraping / Automation**       | **Apify Actors**                                               | LinkedIn & Facebook mentions                         |
| **Official APIs**               | **Google Business, YouTube Data, Reddit API, Facebook Graph**  | Structured review data                               |
| **Scheduler / Background Jobs** | **Celery + Redis (or Apify scheduling)**                       | 8-hour automatic data collection                     |
| **Notifications**               | **Twilio / SMTP**                                              | Email, SMS, WhatsApp alerts                          |
| **Hosting**                     | **Frontend:** Vercel **Backend:** Render **DB:** MongoDB Atlas | Cloud-native deployment                              |
| **CDN & Security**              | **Cloudflare**                                                 | HTTPS, caching, domain protection                    |
| **Version Control / CI/CD**     | **GitHub**                                                     | Source control, automatic deployment                 |

Note: Frontend will use Next.js (not Vite) and backend will use FastAPI (Python) as the primary stack for implementation.

| **Version**   | **Features**                 | **Focus Area**                          | **Technical Domains**            |
| ------------- | ---------------------------- | --------------------------------------- | -------------------------------- |
| **v1**        | 5 Core Modules               | Review Management                       | NLP + Data Engineering           |
| **v2**        | 4 Smart Modules              | Predictive & Analytical Intelligence    | Advanced NLP + ML + Time Series  |
| **v3 (Lite)** | 5 Ethical Engagement Modules | Social Intelligence + Conversational AI | NLP + Ethics + Conversational AI |

---

## 5. **Detailed Feature Breakdown**

### 🧩 **v1 – Core Modules (Foundation)**

#### 1. **Multi-Platform Review Integration**

**Purpose:** Aggregate customer reviews and mentions from all key platforms using a comprehensive hybrid approach.  
**Data Collection Strategy:**

**🔌 Official API Integration (Primary Sources):**

- Google Business Profile API → Reviews & Ratings
- YouTube Data API → Comments & Community Posts
- Reddit API → Mentions & Discussions
- Facebook Graph API → Client's own Facebook Page (reviews, comments, posts)

**🤖 Apify Automation (Secondary Sources):**

- Facebook Public Mentions Scraper → Public posts mentioning business (hashtags, brand mentions)
- LinkedIn Company Page Scraper → Public company mentions and hashtags

**How It Works:**

- 🔄 **APIs:** Fetch structured data every 15 minutes using official APIs for Google Business, YouTube, Reddit, and client's own Facebook Pages.
- 🤖 **Facebook Hybrid:** Uses Graph API for client's own page data (free) + Apify for public mentions/hashtags (paid per run).
- 🕸️ **LinkedIn Apify:** Collects publicly available company mentions via compliant automation that manages proxies, rate limits, and platform restrictions.
- 🗂️ Stores unified data with timestamps, ratings, sentiment, and source platform.
- 📋 Single dashboard shows all reviews and mentions in one consolidated view.

**Example:**

> A café receives a new 2⭐ review on Google, a comment on their own Facebook page, and a public Facebook post saying "Great coffee at [Business Name] but service was slow." All three appear instantly on the unified dashboard with source attribution and cost-optimized data collection.

---

#### **1.1 Facebook Hybrid Data Collection Strategy**

**Purpose:** Optimize Facebook data collection through a dual-approach model that balances cost efficiency with comprehensive coverage.

**The Two Facebook Data Sources:**

| Data Source                    | Access Method         | Cost                | Coverage                                 |
| ------------------------------ | --------------------- | ------------------- | ---------------------------------------- |
| **Client's Own Facebook Page** | ✅ Facebook Graph API | 💰 **Free**         | Reviews, comments, posts, page ratings   |
| **Public Brand Mentions**      | ⚙️ Apify Automation   | 💸 **Paid per run** | Hashtags, brand mentions in public posts |

**Technical Implementation:**

- **Graph API Integration:** OAuth-based connection allowing clients to grant page access tokens for their own Facebook pages.
- **Apify Public Scraping:** Compliant automation for public mentions and hashtag tracking across the broader Facebook network.
- **Cost Optimization:** Up to 70-80% reduction in automation costs by using free Graph API for owned page data.
- **Unified Pipeline:** Both data sources feed into the same MongoDB collection with source attribution.

**Client Experience:**

- **Integrations Page:** Separate options for "Connect Facebook Page" (Graph API) and "Track Public Mentions" (Apify).
- **Dashboard Clarity:** Clear indication of data source (Own Page vs. Public Mentions) for transparency.
- **Pricing Transparency:** Public mention tracking available as premium feature under Professional/Business plans.

**Example Workflow:**

> Restaurant owner connects their Facebook page via Graph API (free). System automatically retrieves all page reviews and comments. Optionally, they enable "Public Mentions" tracking to monitor when customers mention their restaurant in personal posts or food groups (Apify-based, included in Professional plan).

---

#### 2. **Basic Sentiment Classification**

**Purpose:** Understand emotional tone of each review.  
**Method:** Pre-trained multilingual model (Sinhala, Tamil, English).  
**Output:** Positive / Neutral / Negative with confidence score.

**Example:**

> Review: "Food was good, but service was slow."  
> Output: 🍴 Food = Positive (0.88), 🕒 Service = Negative (0.73)

---

#### 3. **AI Response Generator (Human-Approved)**

**Purpose:** Generate empathetic, context-aware replies in local languages.  
**Languages:** Sinhala, Tamil, English.  
**Safety:** All replies require manual approval before posting.

**Example:**

> Review: “Waited 45 minutes for delivery.”  
> Suggested reply: “We’re truly sorry for the delay, [Name]. We’re improving our delivery process and appreciate your patience.”

---

#### 4. **Business Intelligence Dashboard**

**Purpose:** Provide intuitive visual insights for owners.  
**Features:**

- 📈 Rating trend graphs
- 🥧 Sentiment pie charts
- 📊 Review volume over time
- 📤 Exportable reports (PDF/Excel)

**Example:**

> A hotel owner views that 60% of negative reviews mention “WiFi” — identifies a quick fix area.

---

#### 5. **Smart Alert System**

**Purpose:** Notify owners immediately about critical feedback.  
**Triggers:**

- 1⭐/2⭐ reviews
- 📉 Sentiment spikes
- Keywords: “refund”, “complaint”, “bad service”

**Delivery:** WhatsApp, Email, or In-App Notifications.

**Example:**

> “🚨 Alert: 1⭐ Review Detected on Google — ‘Staff was rude.’”

---

### 🧠 **v2 – Smart Intelligence Modules**

#### 6. **Aspect-Based Sentiment Analysis**

**Purpose:** Understand sentiment for specific aspects (Service, Price, Cleanliness, etc.).  
**Tech:** Fine-tuned BERT/XLM-RoBERTa models.

**Example:**

> “Food was delicious, but the waiter was rude.”  
> Output → Food: Positive (0.91), Service: Negative (0.78)

---

#### 7. **Predictive Reputation Analytics**

**Purpose:** Forecast rating trends for the next 1–3 months.  
**Tech:** Prophet/LSTM time-series forecasting.

**Example:**

> “Complaints about ‘delivery delay’ up 35% → predicted 0.2-star drop next month.”

---

#### 8. **Review Plausibility Analysis**

**Purpose:** Assess the credibility and authenticity patterns of reviews.  
**Features:**

- Detect repetitive text patterns
- Identify unusual account behaviors
- Plausibility confidence score

**Example:**

> "Identical 1⭐ reviews from new accounts → Low plausibility (15% confidence)."

---

#### 9️. **Conversational AI Assistant**

**Purpose:** Allow owners to query business insights via natural language.  
**Examples:**

- “Show me negative reviews from last month.”
- “What are the top customer complaints this week?”  
  **Tech:** RAG architecture using vector embeddings for local context.

---

### 💬 **v3 (Lite) – Engagement & Social Intelligence**

#### 10. **Sentiment + Intent Detection**

**Purpose:** Go beyond emotion — understand intent (Complaint, Praise, Query, Request).  
**Example:**

> “Is your store open on Sunday?” → Intent: Query  
> “Your delivery guys are always late” → Intent: Complaint

---

#### 11. **Conversational AI Engagement Bot (with Oversight)**

**Purpose:** Suggest empathetic, pre-approved replies to customer complaints or queries.  
**Safety:** Human review before posting.  
**Example:**

> User: “Terrible service yesterday!”  
> AI Suggests: “We’re truly sorry to hear that. Could you DM us your order details so we can help?”

---

#### 12. **Issue Extraction & Reporting Engine**

**Purpose:** Automatically group similar complaints into categories.  
**Example Output:**

> “This week: 12 delivery issues, 5 refund complaints, 4 staff compliments.”  
> **Tech:** Topic modeling (BERTopic) + summarization (BART).

---

#### 13. **Customer Satisfaction Feedback Loop**

**Purpose:** Follow up to verify issue resolution.  
**Example:**

> “We noticed you reported a delivery issue last week. Has it been resolved?”  
> Tracks customer sentiment improvement over time.

---

#### 14. **Basic Competitor Tracking**

**Purpose:** Monitor the public reputation of key competitors.  
**Features:**

- Track average rating changes for up to 3 competitors.
- Compare review volume and sentiment trends.
- Identify competitor weaknesses to turn into opportunities.

**Example:**

> A café notices a rival’s sentiment for “coffee quality” is dropping, so they launch a marketing campaign focused on their premium beans.

---

## 6. **Real-World Scenarios (Refined & Impactful)**

### 🧋 **Scenario 1 – Local Café Turns Viral Feedback into Growth**

**Problem:** Multiple customers mention "Great coffee, slow service" across Google and Facebook.

**Reputify in Action:**

1. **Aspect Analysis (v2)** identifies "service delay" as a recurring complaint.
2. **Predictive Analytics (v2)** forecasts a 0.3⭐ rating drop if unresolved.
3. **AI Engagement Bot (v3)** suggests an empathetic public reply.
4. **Issue Extraction (v3)** shows 18 similar complaints in a week.
5. **Follow-up Loop (v3)** confirms 40% improvement after process change.

**Result:** The café rebrands around “Fast + Fresh,” gains 150 new 5⭐ reviews in 3 months.

---

### 🏨 **Scenario 2 – Boutique Hotel Enhances Guest Experience with AI Insights**

**Problem:** Reviews say, "Beautiful place, but hard to contact reception."

**Reputify in Action:**

1. **Intent Detection (v3)** flags these as "query + frustration."
2. **Dashboard (v1)** visualizes the spike under the “communication” category.
3. **Predictive Analytics (v2)** shows potential sentiment decline in 2 weeks.
4. **AI Assistant (v2)** recommends automating guest messaging via WhatsApp.
5. **Feedback Loop (v3)** gathers post-fix feedback confirming satisfaction rise.

**Result:** Average rating jumps from 4.1 → 4.7; bookings increase 25%.

---

### 🛍️ **Scenario 3 – Fashion Retail Brand Protects Its Online Image**

**Problem:** Sudden negative sentiment spikes appear across multiple platforms — Google reviews and Facebook mentions.

**Reputify in Action:**

1. **Hybrid Facebook Collection** captures 1⭐ Google reviews + direct comments on brand's Facebook page (Graph API) + negative public Facebook posts mentioning the brand (Apify).
2. **Cost-Optimized Data Pipeline** processes owned page data for free while paying only for public mention analysis.
3. **Review Plausibility (v2)** detects repetitive phrasing patterns across both Facebook data sources → flags potentially coordinated attacks.
4. **Alert System (v1)** instantly notifies the PR manager via WhatsApp with cross-platform evidence and source attribution.
5. **Aspect Sentiment (v2)** isolates "delivery" complaints across all platforms, showing consistent issue pattern vs. isolated fake reviews.
6. **Ethical Engagement Bot (v3)** drafts separate responses: official reply for own page + calm, factual public statement addressing legitimate delivery concerns.

**Result:** Brand responds transparently to real delivery issues while reporting coordinated fake reviews; customer trust actually increases due to proactive communication. Achieves 70% cost reduction in Facebook monitoring compared to pure Apify approach.

---

### 💬 **Scenario 4 – Healthcare Center Builds Patient Trust with Empathetic AI**

**Problem:** Feedback says, "Staff were kind but billing was confusing."

**Reputify in Action:**

1. **Intent = Complaint**, **Aspect = Billing Transparency.**
2. **AI Response Generator (v1)** creates a polite apology with explanation request.
3. **Issue Extraction (v3)** groups billing complaints → triggers internal review.
4. **Follow-up (v3)** confirms resolution via SMS survey.

**Result:** Patient sentiment improves by 40%; hospital highlights “Transparent Care” in marketing.

---

### 🏫 **Scenario 5 – Educational Institute Boosts Reputation Through Transparency**

**Problem:** Students complain on Facebook about "slow response to inquiries."

**Reputify in Action:**

1. **Intent Detection (v3)** classifies these as "queries."
2. **Alert System (v1)** notifies admin staff in real-time.
3. **Dashboard (v1)** shows inquiry-related mentions up by 55%.
4. **Conversational AI (v2)** summarizes frequent issues for management.
5. **Feedback Loop (v3)** measures post-change sentiment.

**Result:** Faster student communication → 25% rise in admissions inquiries and improved online reputation.

---

## 7. **Technical Stack (Social Listening System)**

| **Layer**           | **Tools & Frameworks**               | **Notes**                                          |
| ------------------- | ------------------------------------ | -------------------------------------------------- |
| **Frontend**        | Next.js 14, React 18, Tailwind CSS   | Responsive, modern dashboard UI                    |
| **Backend**         | FastAPI (Python), REST APIs          | High performance, async data collection            |
| **Database**        | MongoDB Atlas (Free Tier)            | Flexible document storage for varied platform data |
| **Data Collection** | Official APIs + Apify Platform       | 7-platform coverage with ethical scraping fallback |
| **ML/NLP**          | HuggingFace Transformers, TextBlob   | Free multilingual sentiment analysis               |
| **AI Processing**   | Open Source Models (BERT, XLM-R)     | Local inference, no API costs                      |
| **Notifications**   | Twilio (SMS), SendGrid (Email)       | Real-time alerts, pay-as-you-go                    |
| **Hosting**         | Vercel (Frontend) + Render (Backend) | Free tier deployment                               |
| **Orchestration**   | Cron Jobs, Background Tasks          | Automated data collection scheduling               |

💰 **Estimated Monthly Cost: $30-40** (mostly Apify usage for platforms without free APIs)

---

## 8. **Ethical Data Collection & Privacy Compliance**

**Reputify's Social Listening Model** follows strict ethical guidelines and only processes publicly available data:

### **🔐 Official API Sources (Primary - 100% Compliant)**

- **Facebook & Instagram Graph APIs:** Client-authorized access to their own business accounts via OAuth
- **Google Places API:** Public business reviews and ratings data
- **YouTube Data API:** Public comments and video content
- **Reddit API:** Public posts and comments in relevant subreddits
- **LinkedIn Marketing API:** Connected company page data with proper authorization

### **🤖 Apify Automation (Secondary - Public Data Only)**

- **TikTok:** Public hashtags, mentions in captions, and comments on public videos
- **LinkedIn:** Public company mentions and professional discussions where API is limited
- **Facebook/Instagram:** Public posts containing brand mentions (not accessible via Graph API)
- **Ethical Standards:** All scraping targets only public, non-personal content
- **Rate Limiting:** Respects platform guidelines and implements proper delays

### **🛡️ Privacy & Security Framework**

- **Public Data Only:** No private messages, personal profiles, or restricted content
- **No Personal Data Storage:** Focus on brand mentions and business-relevant content only
- **GDPR Compliance:** Data minimization, user rights, and proper consent mechanisms
- **Secure Infrastructure:** Encrypted storage, API key protection, and access controls
- **Transparent Disclosure:** Clear communication about data sources and collection methods

### **📋 Operational Boundaries**

1. **What We Collect:** Public mentions, reviews, hashtags, and comments related to client businesses
2. **What We Don't Collect:** Private messages, personal user data, or restricted content
3. **Data Retention:** Configurable retention periods with automatic purging
4. **User Rights:** Data access, correction, and deletion capabilities
5. **Audit Trail:** Complete logging of all data collection and processing activities

> **Privacy-First Approach:** Reputify operates as a social listening platform that processes only publicly available business-related content. All data collection methods comply with platform terms of service, GDPR requirements, and industry best practices for ethical data use.

---

## 9. **SaaS Business Model**

| **Plan**         | **Price (LKR)** | **Platform Coverage**                           | **Target Market**            | **Key Features**                 |
| ---------------- | --------------- | ----------------------------------------------- | ---------------------------- | -------------------------------- |
| **Starter**      | 3,000/month     | Google Reviews + Facebook/Instagram (own pages) | Small cafes, shops           | Basic monitoring, email alerts   |
| **Professional** | 9,000/month     | + YouTube + Reddit + Public social mentions     | Growing restaurants, clinics | SMS alerts, sentiment analysis   |
| **Business**     | 24,000/month    | All 7 platforms (complete coverage)             | Hotel chains, agencies       | Full analytics, priority support |

**Break-even:** 3 customers  
**Scalable Goal:** 200 customers = LKR 1.5M/month

---

## 10. **Research & Innovation Value**

- 🧠 **NLP:** Multilingual sentiment & aspect extraction (Sinhala/Tamil/English).
- 📈 **ML:** Predictive forecasting for customer satisfaction trends.
- 🗣️ **Conversational AI:** Context-aware, empathy-driven communication.
- ⚖️ **Ethics in AI:** Human-in-loop + tone regulation.

**Academic Relevance:**  
Strong cross-domain coverage (NLP + ML + Time-Series + Conversational AI).

---

## 11. **Future Expansion (v3 Full)**

Planned for premium enterprise customers:

- ✅ **Extended Social Media Monitoring:** Expand Apify integration to additional platforms (TikTok, Threads, Instagram Stories) for comprehensive social listening.
- ✅ **Advanced Competitor Intelligence:** Enhanced competitor sentiment tracking across all supported platforms.
- ✅ **AI-Powered Trend Analysis:** Advanced trend visualization with predictive insights and AI coaching recommendations.
- ✅ **Multi-Language Support Expansion:** Extend NLP models to support additional South Asian languages (Malayalam, Telugu, Bengali).
- ✅ **Enterprise API Access:** White-label API for integration with existing business management systems.

**All data collection maintains the same ethical hybrid model:** Official APIs as primary sources, with Apify automation for public social content where APIs are limited.

---

## 12. **Expected Outcomes**

| **Metric**                     | **Target**                     |
| ------------------------------ | ------------------------------ |
| **Sentiment Accuracy**         | >92% (Sinhala/Tamil/English)   |
| **Detection & Response Time**  | <3 minutes for new reviews     |
| **Rating Forecast Accuracy**   | >85% vs. actual trend          |
| **Customer Satisfaction Rate** | +30% improvement over 3 months |

---

## 13. 🧱 **Realistically Buildable in 6 Months**

### ✅ **Must-Have (Fully Buildable MVP)**

**Focus for the first 4 months:**

1.  **Hybrid Review Integration (v1.1)** – Official APIs (Google, YouTube, Reddit, Facebook Graph) + Apify automation setup with unified data pipeline and cost optimization.
2.  **Basic Sentiment Classification (v1.2)** – multilingual model fine-tuned for social media and review content across all 7 platforms.
3.  **AI Response Generator (v1.3)** – LLaMA/Gemini prompt pipeline with approval layer for cross-platform responses.
4.  **Dashboard + Alerts (v1.4, v1.5)** – real-time sentiment charts & WhatsApp/email alerts with Facebook hybrid data integration.
5.  **Aspect-Based Analysis (v2.6)** – fine-tuned XLM-R model with aspect dictionary for multi-platform content including Facebook dual sources.
6.  **Issue Extraction + Reporting (v3.12)** – BERTopic + summarization (BART) for cross-platform pattern detection with source attribution.

💡 These 6 alone deliver a polished, demo-ready SaaS MVP with comprehensive data coverage — real AI + clear business value.

### ⚙️ **Phase 2 (Prototype-Level)**

**Focus during months 4–6:**

7.  **Predictive Analytics (v2.7)** – implement Prophet baseline model.
8.  **Conversational Insights (v2.9)** – simple RAG chatbot querying review DB.
9.  **Intent Detection (v3.10)** – fine-tune small classification head over XLM-R.
10. **Conversational AI Engagement Bot (v3.11)** – empathetic reply suggestions with human approval.
11. **Competitor Tracking (v3.14)** – limited to 1–2 public pages using API/manual entry.

These add clear “startup” value and enhance your academic and innovation score.

### 🧠 **Simulated or Optional (Documented, Not Full Build)**

Can be conceptually demonstrated:

- **Review Plausibility Analysis (v2.8)** – show algorithm logic + synthetic dataset demo.
- **Feedback Loop (v3.13)** – mock email follow-up flow.

## 14. **Conclusion**

**Reputify v3** evolves from a simple review manager to a full-fledged **AI Reputation Intelligence System**.

It helps businesses:

- Listen to customers intelligently.
- Analyze feedback with AI.
- Respond empathetically and ethically.
- Predict and prevent future reputation crises.

> "Businesses don't fail from bad products — they fail from silent customers.  
> Reputify ensures you never miss their voice."

---

### 👥 **Team Reputify - Y3-05**

**Mission:** Empower businesses with AI-driven social intelligence that’s multilingual, ethical, and affordable.  
**Vision:** Become South Asia’s leading AI reputation platform for SMEs.  
**Tagline:** _Listen Smarter. Respond Faster. Grow Stronger._

---
