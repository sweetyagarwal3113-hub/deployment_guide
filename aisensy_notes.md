# 📘 AiSensy – Complete Technical Notes & Platform Comparison

## 1. What is AiSensy?

**AiSensy** is a WhatsApp business communication and automation platform that helps businesses use the **official WhatsApp Business Platform** for:

* WhatsApp marketing & bulk broadcasting
* Customer support & multi-agent live chat
* Visual chatbots & AI WhatsApp agents
* Automated transactional notifications
* Audience segmentation & campaign scheduling
* Link tracking & retargeting
* CRM, E-commerce & API integrations

AiSensy is a **third-party Business Solution Provider (BSP)** layer built around the official WhatsApp Business Platform.

### Simple definition

> **AiSensy is a platform that makes it easier for businesses to automate, manage, and scale WhatsApp communication using the official WhatsApp Business API.**

Official website: [AiSensy](https://aisensy.com/)

---

## 2. WhatsApp Ecosystem Architecture

Before understanding AiSensy, understand the three levels:

```text
                    WhatsApp Ecosystem
                            │
        ┌───────────────────┴───────────────────┐
        │                                       │
 WhatsApp App                     WhatsApp Business App
 (Personal Use)                      (Small Business)
                                            │
                                            │
                                 WhatsApp Business Platform
                                            │
                         ┌──────────────────┴──────────────────┐
                         │                                     │
                  Meta Cloud API                      Providers (BSPs)
                         │                                     │
                         │                         ┌───────────┤
                         │                         │
                  Your Backend                 AiSensy / WATI / Interakt /
                                               Gupshup / Twilio / etc.
```

### Important Architecture Concept

AiSensy **does not replace WhatsApp or Meta**.

```text
Your Application ──> AiSensy ──> Meta WhatsApp Business Platform ──> Customer WhatsApp
```

---

## 3. Normal WhatsApp vs WhatsApp Business App vs AiSensy

| Feature | Normal WhatsApp | WhatsApp Business App | AiSensy (WhatsApp API) |
| ------- | --------------- | --------------------- | ---------------------- |
| Personal messaging | ✅ Yes | ✅ Yes | ❌ Business Only |
| Bulk messaging | ❌ Block risk | Limited (256/list) | ✅ Unlimited Tiers |
| REST API automation | ❌ No | ❌ No | ✅ Full REST API |
| Chatbot Builder | ❌ No | Limited Auto-reply | ✅ Visual Drag-and-drop |
| AI Context Agents | ❌ No | ❌ No | ✅ Built-in AI Agents |
| Multi-agent Inbox | ❌ No | Limited (4-10 devices)| ✅ Unlimited Team Agents |
| Campaign Analytics | ❌ No | Basic | ✅ Real-time Analytics |
| CRM / Webhook Support | ❌ No | ❌ No | ✅ Full Integration |

---

## 4. Comprehensive Alternatives Breakdown

Depending on business domain (E-commerce, Support, Lead Gen, Enterprise, Developer-first), major alternatives to AiSensy offer specialized strengths:

### 1. WATI (WhatsApp Team Inbox)
* **Primary Focus:** Customer support & team inbox ticketing.
* **Key Strengths:** Superior multi-agent inbox UI, granular role permissions, native Shopify integration, automated ticket routing.
* **Best For:** Dedicated customer support teams and growing SMBs.

### 2. Interakt
* **Primary Focus:** E-commerce sales growth & catalogue shopping.
* **Key Strengths:** Automated abandoned cart recovery, cash-on-delivery (COD) verification, seamless Shopify catalogue sync.
* **Best For:** Direct-to-Consumer (D2C) e-commerce brands.

### 3. Gallabox
* **Primary Focus:** No-code bot flows & lead qualification.
* **Key Strengths:** Visual drag-and-drop bot builder, WhatsApp payments, multi-lingual support, seamless bot-to-human handoff.
* **Best For:** Real estate, education, and lead generation businesses.

### 4. Gupshup
* **Primary Focus:** Enterprise API gateway & omnichannel messaging.
* **Key Strengths:** High messaging throughput, multi-channel support (WhatsApp, SMS, RCS, Instagram), custom enterprise integrations.
* **Best For:** Large enterprise corporations, banks, and fintech platforms.

### 5. Twilio
* **Primary Focus:** Developer-first communications API infrastructure.
* **Key Strengths:** Complete programmatic API control, global reliability, pay-as-you-go pricing without mandatory UI subscriptions.
* **Best For:** Engineering teams building custom SaaS applications from scratch.

### 6. Respond.io
* **Primary Focus:** Omnichannel customer conversation management.
* **Key Strengths:** Unifies WhatsApp, Facebook Messenger, Telegram, Instagram DM, Viber & Webchat into a single inbox.
* **Best For:** Global businesses operating across multiple chat channels.

### 7. Doubletick
* **Primary Focus:** Mobile-first WhatsApp marketing & CRM.
* **Key Strengths:** Ultra-fast mobile app interface, broadcast scheduling, contact management, sales tracking.
* **Best For:** Sales teams and mobile-first business owners.

### 8. BiteSpeed
* **Primary Focus:** Shopify WhatsApp marketing & revenue recovery.
* **Key Strengths:** Segmented broadcast campaigns, pop-up opt-in tools, review collection, upsell/cross-sell bots.
* **Best For:** Shopify e-commerce brands.

### 9. Yellow.ai / LimeChat
* **Primary Focus:** Enterprise AI Agent automation.
* **Key Strengths:** Generative AI conversational agents, deep ERP/CRM backend integration, autonomous multi-turn reasoning.
* **Best For:** High-volume enterprise customer support automation.

---

## 5. Master Platform Alternatives Comparison Matrix

| Platform | Target Audience | Primary Strength | Pricing Model | Chatbot Type |
| -------- | --------------- | ---------------- | ------------- | ------------ |
| **AiSensy** | SMBs & Marketers | Broadcasting, Retargeting & AI Agents | Monthly Sub + Meta Fees | Drag-and-Drop + AI Agent |
| **WATI** | Support Teams | Multi-agent team inbox | Monthly Sub + Meta Fees | Rule-based Bot |
| **Interakt** | Shopify D2C Brands | Abandoned Cart & Catalogues | Monthly Sub + Meta Fees | E-commerce Rule Bot |
| **Gallabox** | Lead Generation | WhatsApp Payments & Regional Bots | Monthly Sub + Meta Fees | Visual Flow Builder |
| **Gupshup** | Enterprise Companies | Massive throughput & Omnichannel API | Custom Enterprise Plan | AI Studio / Custom API |
| **Twilio** | Developers | Raw Programmable API infrastructure | Pay-as-you-go per Msg | Custom Backend Logic |
| **Respond.io** | Global Omnichannel | Unified Inbox (WhatsApp+Insta+Telegram) | Tiered User Seats | Workflow Automations |
| **Doubletick** | Mobile Sales Teams | Mobile App Broadcast & CRM | Monthly Sub + Meta Fees | Basic Auto-replies |
| **BiteSpeed** | Shopify E-commerce | Revenue Recovery & Review Collection | Monthly Sub + Meta Fees | E-com Marketing Bot |

---

## 6. Main Features of AiSensy

* **WhatsApp Broadcasting:** Personalized bulk broadcasts with variables.
* **Audience Segmentation:** Filter users by location, purchase history, or custom tags (`VIP`).
* **Retargeting:** Automatically trigger follow-up campaigns to users who clicked links in previous broadcasts.
* **Chatbot Builder:** Visual tree builder for quick replies and FAQs.
* **AI WhatsApp Agents:** Context-aware NLU agents that understand freeform user intent.
* **Multi-Agent Live Chat:** Shared inbox for team collaboration and support handoff.
* **Click-to-WhatsApp Ads (CTWA):** Route traffic from Meta ads straight into WhatsApp chats.

---

## 7. WhatsApp Templates & Meta Policies

### 1. Template Messages
Business-initiated messages MUST use pre-approved Template Messages containing parameters (e.g., `Hello {{1}}, your order {{2}} has been shipped`).

### 2. Template Categories
* **Marketing:** Promotional offers, sales, product launches.
* **Utility:** Order updates, appointment reminders, transaction receipts.
* **Authentication:** OTPs and verification codes.

### 3. The 24-Hour Customer Service Window
* **Inside 24-hr Window:** Triggered when a user sends a message. Business can reply with free-form text, images, and custom messages for FREE. Every user message resets the 24-hour clock.
* **Outside 24-hr Window:** Business can ONLY send pre-approved Template Messages.

### 4. Messaging Limits & Quality Score
Meta enforces messaging tiers based on account quality:
* Tier 1: 1,000 unique users / 24 hrs
* Tier 2: 10,000 unique users / 24 hrs
* Tier 3: 100,000 unique users / 24 hrs
* Tier 4: Unlimited unique users

---

## 8. Backend Pipeline & System Architecture

A production WhatsApp backend pipeline consists of:

```text
[ Database ] ──> [ Cron Scheduler ] ──> [ Backend Gateway ] ──> [ AiSensy REST API ] ──> [ Meta Cloud API ] ──> [ User WhatsApp ]
```

### Key Architectural Rules:
1. **Idempotency:** Maintain a composite constraint (`user_id + notification_type + scheduled_date`) to prevent duplicate dispatches during server restarts.
2. **Security:** Store API keys in server-side environment variables (`.env`). Never expose credentials on the client side.

---

## 9. Webhooks & Event-Driven Architecture

A **Webhook** is an HTTP POST notification sent by AiSensy/Meta to your backend server when an asynchronous event occurs.

### Supported Event Statuses:
* `sent`: Accepted by Meta servers.
* `delivered`: Received on destination device.
* `read`: Opened by user.
* `incoming_message`: User responded with text/media.

### API vs Webhook Comparison:
* **API (Outbound):** Your system requests an action from AiSensy (Command).
* **Webhook (Inbound):** AiSensy notifies your system of an event (Push Notification).

---

## 10. Pricing Structure

Total Cost = **AiSensy Subscription Fee** + **Meta Conversation Charges**

### Standard Meta Category Rates (India Recipient Reference):
* **Marketing:** ~₹1.09 / message
* **Utility:** ~₹0.145 / message
* **Authentication:** ~₹0.145 / message
* **Service:** Free inside 24-hr service window

---

## 11. Key Terminology Glossary

* **WABA:** WhatsApp Business Account.
* **BSP:** Business Solution Provider (e.g., AiSensy, WATI, Interakt).
* **CTWA:** Click-to-WhatsApp Ads.
* **Template:** Meta pre-approved message format required outside 24-hr window.
* **24-Hour Window:** Customer service timeframe triggered by incoming user message.
* **Opt-In:** Explicit user consent required prior to business messaging.

---

## 12. Architectural Summary Cheat Sheet

```text
OUTBOUND:  DB ──> Scheduler ──> Backend ──> AiSensy API ──> Meta ──> User WhatsApp
INBOUND:   User WhatsApp ──> Meta ──> AiSensy ──> Webhook Endpoint ──> DB Update
PRO TIP:   Select provider based on domain: AiSensy (Marketing/AI), WATI (Support), Interakt (Shopify), Twilio (Developer API)!
```
