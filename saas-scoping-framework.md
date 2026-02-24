# SaaS Application Scoping Framework for Claude Code

## Overview

This framework helps non-technical founders systematically plan SaaS applications before development. By answering these questions and following this process, you'll create clear, actionable instructions for Claude Code to build your application effectively.

---

## Phase 1: Feature Planning & Prioritization

### 1.1 Core Features (MVP)

List only the absolute essential features needed to solve the core problem:

1. **Feature Name**
   - What it does
   - Why it's essential
   - Success criteria

2. **Feature Name**
   - What it does
   - Why it's essential
   - Success criteria

### 1.2 User Journey Mapping

For each core feature, describe the user flow:

**Example Format:**
```
Feature: User Registration
1. User clicks "Sign Up"
2. User enters email and password
3. System sends verification email
4. User clicks verification link
5. User is logged in and sees dashboard
```

### 1.3 Future Features (Post-MVP)

- Phase 2 features (nice-to-have)
- Phase 3 features (growth features)
- "Someday" features (vision features)

---

## Phase 2: Technical Requirements & Constraints

### 2.1 Data & Storage

- **What data will you store?**
  - User data
  - Application data
  - Files/media

- **Data relationships**
  - How do different data types connect?
  - What needs to be linked together?

### 2.2 User Access & Permissions

- **User Types**
  - Admin
  - Regular user
  - Guest
  - Custom roles?

- **Permissions Matrix**

```
| Feature   | Admin | User | Guest |
|-----------|-------|------|-------|
| View X    | Yes   | Yes  | No    |
| Edit X    | Yes   | No   | No    |
```

### 2.3 Integration Requirements

- **External Services**
  - Payment processing (Stripe, PayPal?)
  - Email service (SendGrid, Postmark?)
  - Analytics (Google Analytics, Mixpanel?)
  - Storage (AWS S3, Cloudinary?)

- **API Needs**
  - Will others need to access your data?
  - Do you need to connect to other tools?

### 2.4 Performance & Scale

- **Expected Usage**
  - Number of users (launch, 6 months, 1 year)
  - Concurrent users
  - Data volume

- **Response Time Requirements**
  - Page load expectations
  - Critical operations that must be fast

---

## Phase 3: User Experience Design

### 3.1 Interface Principles

- **Design Style**
  - Modern/minimal
  - Professional/corporate
  - Friendly/casual
  - Technical/developer-focused

- **Key UI Elements**
  - Navigation style (sidebar, top nav, etc.)
  - Mobile responsiveness priority
  - Accessibility requirements

### 3.2 Information Architecture

- **Main Sections**
  - Dashboard
  - Settings
  - User management
  - [Your specific sections]

- **Navigation Hierarchy**

```
Home
├── Dashboard
├── Feature 1
│   ├── Sub-feature A
│   └── Sub-feature B
└── Settings
```

### 3.3 Key Pages/Screens

For each major screen, describe:
- Purpose
- Key information displayed
- Main actions available
- Success metrics

---

## Phase 4: Business Model & Monetization

### 4.1 Pricing Strategy

- **Model Type**
  - Subscription (monthly/annual)
  - One-time purchase
  - Freemium
  - Usage-based

- **Pricing Tiers**
  - Free/Trial: [features]
  - Basic: $X/month [features]
  - Pro: $X/month [features]
  - Enterprise: Custom [features]

### 4.2 Payment & Billing

- **Payment Methods**
  - Credit card
  - PayPal
  - Invoice

- **Billing Features**
  - Trial period length
  - Upgrade/downgrade rules
  - Refund policy

---

## Phase 5: Success Metrics & Analytics

### 5.1 Key Performance Indicators (KPIs)

- **User Metrics**
  - Sign-ups
  - Active users
  - Churn rate

- **Business Metrics**
  - MRR (Monthly Recurring Revenue)
  - Customer Lifetime Value
  - Customer Acquisition Cost

### 5.2 Analytics Implementation

- **What to Track**
  - User actions
  - Feature usage
  - Error rates
  - Performance metrics

---

## Phase 6: Risk Assessment & Mitigation

### 6.1 Technical Risks

- Data loss → Backup strategy
- Security breaches → Security measures
- Downtime → Monitoring and alerts
- Scaling issues → Architecture planning

### 6.2 Business Risks

- Low adoption → Marketing strategy
- High churn → User feedback loops
- Competition → Differentiation strategy

---

## Phase 7: Development Approach

### 7.1 Technology Decisions

- **Frontend Framework**: React, Vue, or Next.js?
- **Backend**: Node.js, Python, or full-stack framework?
- **Database**: PostgreSQL, MySQL, or MongoDB?
- **Hosting**: Vercel, AWS, or Heroku?

### 7.2 Development Phases

1. **Phase 1**: Core functionality (2-4 weeks)
2. **Phase 2**: User management & auth (1-2 weeks)
3. **Phase 3**: Payment integration (1-2 weeks)
4. **Phase 4**: Polish & testing (1-2 weeks)

---

## Output Template for Claude Code

After completing the above framework, create this structured brief for Claude:

```markdown
# Project Brief: [Your App Name]

## Executive Summary
[2-3 sentences describing what you're building and why]

## Problem & Solution
- **Problem**: [Clear problem statement]
- **Solution**: [How your app solves it]
- **Target Users**: [Who will use this]

## Core Features (MVP)
1. **[Feature 1]**
   - Description: [What it does]
   - User Flow: [Step-by-step process]
   - Success Criteria: [How we know it works]

2. **[Feature 2]**
   - Description: [What it does]
   - User Flow: [Step-by-step process]
   - Success Criteria: [How we know it works]

## Technical Requirements
- **Database Schema**:
  - Users table: [fields]
  - [Other tables]: [fields]
- **Authentication**: [Requirements]
- **Integrations**: [List external services]
- **Performance**: [Key requirements]

## Design Guidelines
- **Style**: [Design direction]
- **Key Pages**: [List with descriptions]
- **Mobile**: [Responsive requirements]

## Business Logic
- **User Roles**: [Define each role]
- **Permissions**: [Who can do what]
- **Pricing**: [If applicable]

## Success Metrics
- [Metric 1]: [Target]
- [Metric 2]: [Target]

## Development Priorities
1. [Most important feature/functionality]
2. [Second priority]
3. [Third priority]

## Constraints & Considerations
- [Any specific limitations]
- [Important business rules]
- [Compliance requirements]
```

---

## Best Practices for Working with Claude Code

### 1. Start Small
- Begin with the simplest version of your core feature
- Test and validate before adding complexity
- Iterate based on what you learn

### 2. Be Specific
- Use concrete examples instead of abstract descriptions
- Provide sample data when possible
- Include edge cases and error scenarios

### 3. Think in User Stories
- "As a [user type], I want to [action] so that [benefit]"
- This helps Claude understand context and purpose

### 4. Provide Visual References
- Sketch simple wireframes
- Share examples of similar apps you like
- Describe the visual hierarchy

### 5. Define Success Clearly
- What does "working" mean for each feature?
- How will you test if it's successful?
- What are the acceptance criteria?

### 6. Communicate Constraints
- Budget limitations
- Timeline requirements
- Technical preferences
- Scaling expectations

---

## Common Pitfalls to Avoid

1. **Feature Creep**: Trying to build everything at once
2. **Vague Requirements**: "Make it user-friendly" without specifics
3. **Ignoring User Feedback**: Building in isolation
4. **Over-Engineering**: Complex solutions for simple problems
5. **Under-Specifying**: Not enough detail for Claude to execute

---

## Next Steps

1. **Complete this framework** for your specific app idea
2. **Create the output brief** using the template
3. **Review and refine** — sleep on it and revisit
4. **Start with Claude Code** on the simplest feature first
5. **Iterate and improve** based on results

Remember: The clearer your vision and requirements, the better Claude Code can help you build it. Take time in the planning phase to save time in development.
