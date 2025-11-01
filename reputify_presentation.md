# REPUTIFY - 5 MINUTE SPEECH
## Easy Read Version (Just Look & Speak)

---

**OPENING**

Good evening sir. I hope you're keeping well.

Today, I'd like to give an update about our project called **Reputify**. 

This idea was approved by Mr. Suresh about two weeks ago, and since then we've been actively developing it step by step.

---

**THE PROBLEM**

Let me start by explaining the problem we're solving.

Today, almost every business depends on online platforms. Google Reviews. Facebook. Instagram. YouTube. Reddit.

Customers share their opinions publicly. They complain publicly. They appreciate publicly.

And other customers read all of that before deciding whether to visit that business or not.

But business owners face three major issues:

**One** - They don't have time to check all platforms every single day.

**Two** - Negative comments go unnoticed. By the time they see it, the damage is already done.

**Three** - Feedback is scattered everywhere. Google says one thing. Facebook says another. They never get the complete picture. They can't understand what's causing their reputation to go up or down.

Because of this, businesses become reactive instead of proactive. They only respond after customers start leaving.

This is a serious blind spot in today's digital world.

---

**OUR SOLUTION**

That's where Reputify comes in.

Reputify is an AI-powered reputation intelligence system.

In simple words, we help businesses:

- **Listen** to what customers say
- **Understand** how customers feel  
- **Respond** faster
- **Improve** reputation with data-driven decisions

We collect reviews from multiple platforms and bring everything into one dashboard.

Our system automatically analyzes sentiment. Positive, negative, or neutral.

It shows reputation trends with clear visuals.

If something urgent happens - like a one-star review or a sudden spike in complaints - the business owner gets an immediate alert on their phone.

They can take action before reputation gets damaged.

We also use AI to suggest professional reply messages. In English, Sinhala, or Tamil.

The owner can review it and send it. This saves time and maintains a consistent brand image.

These replies are human-approved, so the business stays in control.

Our overall flow is simple:

**Monitor → Analyze → Take Action → Improve Reputation**

---

**TECHNICAL IMPLEMENTATION**

Now let me explain how we're building this technically.

Our system has four main components.

**First - Data Collection Layer**

We use a hybrid approach.

For platforms like Google, Facebook, Instagram, YouTube, and Reddit - we use their official APIs.

For platforms without good APIs - like TikTok or public LinkedIn posts - we use web scraping tools like Apify.

This gives us reliability, low cost, and legal compliance. We only collect public data.

We run scheduled cron jobs every three to six hours to automatically fetch new data.

**Second - Backend and Processing Engine**

Our backend is built with FastAPI using Python.

This gives us high performance, easy integration with AI libraries, and async processing for handling multiple platforms simultaneously.

We use MongoDB Atlas as our database.

Why MongoDB? Because it handles unstructured review data very well. It's easy to scale. And it has a flexible schema for different platform formats.

All collected data goes through our AI pipeline which performs:

- Sentiment analysis - classifying positive, negative, or neutral
- Aspect-based analysis - identifying specific topics like food quality, service speed, pricing
- Trend detection - spotting patterns over time
- Urgency classification - flagging critical issues

**Third - AI and NLP Implementation**

This is the core technical innovation.

We're implementing multilingual NLP models specifically trained for Sinhala, Tamil, and English.

We use transformer-based models from HuggingFace.

We're fine-tuning pre-trained models on local business review datasets.

For AI-generated replies, we use GPT-based language models to generate appropriate responses.

We also have template-based fallbacks for reliability.

And we have human-in-the-loop approval before any reply is sent.

The key challenge is handling code-switching. That's when people mix Sinhala and English in one sentence. Our models need to understand that correctly.

**Fourth - Frontend and User Experience**

Our dashboard is built with Next.js and React.

It features:

- Real-time data visualization with charts
- Platform-wise breakdown of reviews
- Sentiment distribution graphs
- AI-suggested action items
- One-click reply functionality

For real-time alerts, we're integrating:

- Email notifications via SendGrid
- WhatsApp alerts via Twilio API
- Push notifications for mobile in future phases

**Our Complete Tech Stack**

Let me summarize our technology stack:

Frontend: Next.js, React, Tailwind CSS

Backend: FastAPI with Python, MongoDB Atlas

AI and ML: HuggingFace Transformers, PyTorch

APIs: Google My Business, Facebook Graph, Instagram Business, YouTube Data, Reddit

Web Scraping: Apify

Hosting: Vercel for frontend, AWS or Render for backend

Notifications: SendGrid for email, Twilio for WhatsApp

Task Scheduling: Celery with Redis

---

**WHY SRI LANKA NEEDS THIS**

Now, why is this important for Sri Lanka?

Most small and medium businesses here don't have tools like this.

They depend on checking one platform manually.

International solutions like Brand24 or Mention are too expensive for local businesses.

But Sri Lankan businesses need support in improving their online trust and brand image.

Reputify is designed to be:

- Affordable
- Easy to use
- Focused on our region's needs
- Supports multiple languages

This last point is crucial. Most global tools don't handle Sinhala and Tamil properly. We do.

When a business manages reputation well online, it directly increases:

- Customer trust
- Sales
- Brand image  
- Long-term success

---

**PROGRESS UPDATE**

Let me share what we've completed so far since approval:

✓ Finalized the name Reputify

✓ Designed our logo

✓ Purchased the domain reputify.lk

✓ Built a marketing website

✓ Started group documentation

✓ Completed system architecture design

✓ Researched and tested API integrations

✓ Started building the data collection pipeline

**Next steps:**

We're moving into wireframing next.

Then we'll implement the core sentiment analysis module.

Build the data collection service.

Set up the database and backend APIs.

Develop the frontend dashboard.

And test with real business data.

We're continuously improving by discussing technical challenges, AI accuracy requirements, and checking what real businesses need.

So we can actually launch this as a real SaaS product someday.

---

**CONCLUSION**

In summary, Reputify is not just a university project.

It's a practical solution to a real-world problem. Businesses losing control of their online reputation.

From a business perspective - we help companies understand customers better, respond faster, and build stronger digital presence.

From a technical perspective - we're building a scalable, AI-powered platform. We're solving real challenges in multilingual sentiment analysis, real-time data processing, and actionable intelligence.

Reputation today is not something businesses can ignore.

It's a major deciding factor for customers.

Thank you sir. That's our update.

We're open to any suggestions or feedback to improve this further.

---

## QUICK REFERENCE

**If short on time, hit these points:**
1. Problem: Reviews scattered, businesses reactive
2. Solution: AI-powered unified dashboard
3. Tech: FastAPI + MongoDB + HuggingFace NLP
4. Unique: Multilingual (Sinhala/Tamil/English)
5. Progress: Domain purchased, architecture done, building pipeline

**Speaking time:** 5-6 minutes at natural pace

**Pause points:** After each major section (marked with ---)