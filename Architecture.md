# Architecture: InsightPulse

## Overview

InsightPulse is designed as an AI-assisted customer feedback intelligence dashboard. The system takes customer reviews as input, processes them through a feedback triage workflow, updates dashboard metrics, and generates an AI-powered product summary.

---

## High-Level Flow

```text
Customer Review Input
        ↓
Feedback Processing Layer
        ↓
Sentiment + Category + Urgency Classification
        ↓
Customer Review Data Store
        ↓
Dashboard Metrics + Recent Review Feed
        ↓
AI Dashboard Summary Agent
        ↓
Product Insight Summary
```

---

## 1. Input Layer

Feedback can enter the system through:

- Manual review submission
- Mock data import
- Future CSV upload
- Future support-ticket or app-review integrations

Current MVP focus:

- Public-facing review submission
- Mock review data for demo testing

---

## 2. Data Model

A customer review record may include:

```text
customer_name
review_text
rating
sentiment
category
urgency_status
created_at
```

Example classification fields:

- `sentiment`: Positive, Neutral, Negative
- `category`: Bug, Feature Request, UI/UX, Performance
- `urgency_status`: Normal or Urgent

---

## 3. AI Triage Workflow

The AI triage workflow acts as a first-pass analysis layer for incoming feedback.

### Step 1: Sentiment Classification

The review text is analyzed and labeled as:

- Positive
- Neutral
- Negative

### Step 2: Category Detection

The review is grouped into a product-related category:

- Bug
- Feature Request
- UI/UX
- Performance

### Step 3: Urgency Detection

The system checks for high-severity terms such as:

- crash
- broken
- failed
- error
- lost money
- cannot use
- system down

If high-severity language is detected, the review is marked as urgent.

---

## 4. Dashboard Layer

The dashboard converts processed review data into product health signals.

Dashboard outputs include:

- Total review count
- Sentiment distribution
- Top product categories
- Recent review feed
- Urgent issue visibility
- AI-generated product summary

---

## 5. AI Dashboard Summary Agent

The AI summary agent reviews dashboard-level signals and generates a concise product brief.

The agent considers:

- Overall sentiment
- Most frequent categories
- Recent negative reviews
- Urgent issue flags
- Product areas needing attention

Output:

- Plain-language product summary
- Key risks
- Positive trends
- Recommended focus areas

---

## 6. Technical Stack

This prototype was created using Base44 as an AI-assisted development platform.

Conceptual technical stack:

- React-style single-page application
- Responsive dashboard UI
- Customer review data model
- AI-assisted classification workflow
- Dashboard analytics layer
- AI summary generation layer
- Public preview access for portfolio review

---

## 7. Future Architecture Enhancements

Future versions could include:

- CSV upload pipeline
- REST API ingestion
- Zendesk, Intercom, Jira, or Azure DevOps integrations
- Confidence scores for AI labels
- Human review and correction flow
- Role-based access control
- Audit logs
- Multi-tenant workspace support
