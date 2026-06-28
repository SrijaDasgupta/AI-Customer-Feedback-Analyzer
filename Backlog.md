# Backlog: InsightPulse

## Epic 1: Customer Feedback Submission

### User Story 1

As a user, I want to submit a customer review so that the system can analyze feedback and add it to the dashboard.

**Acceptance Criteria:**

- User can enter customer name.
- User can enter review text.
- User can add a star rating.
- Submitted review appears in the recent reviews feed.

### User Story 2

As a stakeholder, I want to import mock data so that I can quickly test the dashboard without manually entering reviews.

**Acceptance Criteria:**

- User can trigger mock data import.
- Sample reviews appear in the dashboard.
- Dashboard metrics update after import.

---

## Epic 2: AI Feedback Triage

### User Story 1

As a Product Manager, I want reviews to be classified by sentiment so that I can quickly understand customer satisfaction.

**Acceptance Criteria:**

- Each review receives a Positive, Neutral, or Negative label.
- Sentiment labels are visible in the review feed.
- Dashboard metrics reflect sentiment distribution.

### User Story 2

As a Product Manager, I want reviews categorized by product theme so that I can identify the most common issue areas.

**Acceptance Criteria:**

- Reviews are assigned to categories such as Bug, Feature Request, UI/UX, or Performance.
- Categories are visible in the dashboard or review feed.
- Dashboard metrics reflect category distribution.

### User Story 3

As an Engineering Lead, I want urgent reviews to be flagged so that I can respond faster to critical issues.

**Acceptance Criteria:**

- Reviews mentioning severe issues are marked urgent.
- Urgent reviews are visible in the dashboard or review feed.
- Urgent classification considers terms such as crash, broken, failed, error, or major impact.

---

## Epic 3: Product Health Dashboard

### User Story 1

As a Product Manager, I want to view dashboard metrics so that I can understand product health at a glance.

**Acceptance Criteria:**

- Dashboard shows total reviews.
- Dashboard shows sentiment breakdown.
- Dashboard shows product categories.
- Dashboard shows recent reviews.

### User Story 2

As a Customer Success user, I want to see recent reviews so that I can understand customer concerns quickly.

**Acceptance Criteria:**

- Recent reviews are listed clearly.
- Each review includes rating, sentiment, and category.
- Negative or urgent feedback is easy to identify.

---

## Epic 4: AI Dashboard Summary Agent

### User Story 1

As a Product Manager, I want an AI-generated summary of the dashboard so that I can quickly understand key trends.

**Acceptance Criteria:**

- AI agent reads dashboard-level signals.
- Summary includes sentiment trends.
- Summary highlights urgent issues.
- Summary identifies recommended product focus areas.

### User Story 2

As an Engineering Lead, I want the summary to call out urgent technical issues so that I can prioritize fixes.

**Acceptance Criteria:**

- Summary mentions urgent bug or performance patterns.
- Summary is concise and easy to understand.
- Summary supports faster product and engineering alignment.

---

## Epic 5: Future Integrations

### User Story 1

As a Product Manager, I want to upload a CSV file so that I can analyze feedback from external sources.

**Acceptance Criteria:**

- User can upload a CSV file.
- Required fields are validated.
- Imported reviews appear in the dashboard.

### User Story 2

As an Engineering Lead, I want urgent feedback to create a Jira or Azure DevOps ticket so that engineering action can start quickly.

**Acceptance Criteria:**

- Urgent review can be converted into a ticket.
- Ticket includes review text, category, sentiment, and urgency status.
- Ticket creation status is visible to the user.

---

## Epic 6: AI Governance

### User Story 1

As a user, I want to see confidence scores so that I can understand how reliable the AI classification is.

**Acceptance Criteria:**

- Sentiment and category labels include confidence scores.
- Low-confidence outputs are clearly marked.
- Users can review uncertain classifications.

### User Story 2

As a user, I want to correct AI labels so that the system can improve over time.

**Acceptance Criteria:**

- User can edit sentiment label.
- User can edit category label.
- Corrections are stored for future review.
