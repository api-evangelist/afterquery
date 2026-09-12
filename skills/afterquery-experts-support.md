---
name: Afterqueryexperts
description: Use when helping contributors understand contract work, complete onboarding, manage payments, follow work guidelines, and troubleshoot platform issues. Reach for this skill when agents need to guide users through task completion, quality standards, payment setup, or technical support.
metadata:
    mintlify-proj: afterqueryexperts
    version: "1.0"
---

# AfterQuery Experts

## Product summary

AfterQuery Experts is a contract-based platform where independent contributors complete AI training data annotation tasks—labeling text, images, audio, and other content to train machine learning models. Contributors work flexibly, accept tasks based on their skills, and receive weekly payments via Stripe. The platform handles onboarding (legal documents, identity verification, payment setup), task assignment, quality review, and payout processing. Primary documentation: https://docs.afterquery.com

**Key files and concepts:**
- Onboarding: Four sequential steps (Sign Legal, Verify Phone, Verify Identity, Set Up Payments)
- Payment: Weekly Friday payouts via Stripe; Monday–Sunday work week; 7-day hold on first payout
- Work types: Text classification, sentiment analysis, named entity recognition, image annotation
- Quality evaluation: Accuracy, consistency, completeness, timeliness, communication
- Contract status: Independent contractor (self-employed, flexible scheduling, performance-based pay)

## When to use

Reach for this skill when:
- A user is onboarding and needs help with legal documents, phone/identity verification, or Stripe payment setup
- A contributor is unclear about work guidelines, quality standards, or how to approach specific annotation tasks
- Someone needs to understand payment timing, payout schedules, or troubleshoot payment issues
- A user encounters platform bugs or technical problems and needs troubleshooting steps
- A contributor wants to know about contract terms, task assignment, or performance expectations
- Someone is asking about tax obligations, payment records, or contractor responsibilities

Do not use this skill for: Account creation, application approval decisions, or policy exceptions.

## Quick reference

### Onboarding steps (in order)
| Step | What it does | Key detail |
|------|-------------|-----------|
| Sign Legal | Contractor agreement | Must complete before proceeding |
| Verify Phone | Confirm phone number via Persona | 4-digit code sent by text |
| Verify Identity | Government ID + selfie via Persona | Must match account name exactly; blurry/expired photos rejected |
| Set Up Payments | Create Stripe account | Choose Individual or Business; select country carefully (can't change later) |

### Payment schedule
- **Pay day:** Every Friday by 11:59 p.m. PT
- **Work week:** Monday–Sunday
- **First payout:** 7-day hold from Stripe (mandatory)
- **Subsequent payouts:** 2–3 business days after Friday release
- **Currency:** USD; converted to local currency at payout
- **Method:** Stripe only (bank account required; no cards)

### Work quality metrics
Contributors are evaluated on:
- **Accuracy** — Correctness of annotations
- **Consistency** — Uniform application of guidelines across similar tasks
- **Completeness** — Thoroughness and all required elements addressed
- **Timeliness** — Meeting deadlines for accepted tasks
- **Communication** — Clear, professional interaction with support

### Common annotation task types
| Task type | Focus | Key principle |
|-----------|-------|---------------|
| Text classification | Categorizing content | Choose most specific category; flag unclear cases |
| Sentiment analysis | Emotion/tone labeling | Consider context, sarcasm, cultural factors; avoid personal bias |
| Named entity recognition | Identifying people, places, organizations | Be consistent with format; handle ambiguity; flag unclear cases |
| Image annotation | Labeling objects, drawing bounding boxes | Be precise; account for occlusion and scale; label all relevant objects |

### Troubleshooting quick fixes (in order of effectiveness)
1. Hard refresh: Cmd+Shift+R (Mac) or Ctrl+Shift+R (Windows)
2. Clear cache and cookies (Settings > Privacy > Clear browsing data)
3. Try incognito window or disable browser extensions
4. Turn off VPN (breaks identity verification and payment setup)
5. Switch to desktop browser if mobile upload fails
6. Check spam folder for @afterquery.com emails; add to contacts

## Decision guidance

### When to accept vs. decline a task
| Situation | Action |
|-----------|--------|
| Task matches your skills and you have time | Accept — builds reputation and unlocks better opportunities |
| Task is unclear or guidelines are confusing | Decline or ask for clarification before accepting |
| You're unsure about quality standards | Decline — ask support for examples first, then accept similar tasks later |
| Task deadline conflicts with availability | Decline — you can't extend deadlines once accepted |
| You've completed similar tasks successfully | Accept — consistency improves quality ratings |

### Stripe account setup: Individual vs. Business
| Choice | Use when | Consequence |
|--------|----------|------------|
| **Individual** | You're self-employed with no registered business | Most common; use your personal legal name and bank account |
| **Business** | You have a registered business with its own bank account | Requires business registration; use business bank account |

**Critical:** Country selection is permanent. Verify before continuing.

### Payment delays: Diagnosis
| Symptom | Likely cause | Fix |
|---------|-------------|-----|
| Payout on hold or manual review | Bank account country ≠ profile location | Update profile location to match bank account country |
| Payout went to wrong account | Bank details changed after payout sent | Wait 10–15 business days; money returns to Stripe balance and retries |
| Payout missing from Stripe | Work not yet approved | Payouts cover only approved work; unapproved hours shift to next week |
| First payout delayed 7+ days | Stripe first-payout hold | Mandatory; every payout after the first follows normal Friday schedule |

## Workflow

### Helping a contributor complete onboarding
1. **Confirm current step:** Ask which step they're on (Sign Legal, Verify Phone, Verify Identity, Set Up Payments)
2. **Gather requirements:** Have them check they have government ID, phone that receives texts, and bank account details nearby
3. **Walk through the step:**
   - **Sign Legal:** Confirm they've read and accepted the contractor agreement
   - **Verify Phone:** Confirm Persona window opened, code arrived, and they entered it correctly
   - **Verify Identity:** Confirm ID type matches their document, name on account matches ID exactly, and selfie was clear (not blurry/screenshot)
   - **Set Up Payments:** Confirm they chose the right business type (usually Individual) and country (permanent choice)
4. **Troubleshoot if stuck:** Use quick fixes (hard refresh, clear cache, try incognito, disable VPN)
5. **Escalate if needed:** If Persona verification fails repeatedly or Stripe rejects identity, direct to support@afterquery.com with email, step, and screenshot

### Helping a contributor understand work guidelines
1. **Identify the task type:** Ask what kind of annotation they're doing (text, image, sentiment, entity recognition, etc.)
2. **Review the core principle:** Explain accuracy > speed; consistency across similar tasks is critical
3. **Walk through the checklist:** Before submitting, they should verify:
   - [ ] Followed all instructions exactly
   - [ ] Work is consistent with similar tasks
   - [ ] Considered all relevant factors
   - [ ] No errors or inconsistencies
   - [ ] Flagged any problematic content
   - [ ] Work is complete and thorough
4. **Address quality concerns:** If feedback shows low accuracy or inconsistency, have them review examples of similar tasks and ask for clarification on ambiguous guidelines
5. **Reinforce improvement:** Higher quality work leads to priority access, bonuses, and more complex tasks

### Troubleshooting a payment issue
1. **Confirm the payout status:** Ask them to check their Stripe dashboard or Earnings dashboard for the payout date and status
2. **Identify the problem:** Use the diagnosis table above to match their symptom to a cause
3. **Apply the fix:**
   - **Location mismatch:** Update profile location to match bank account country
   - **Wrong bank details:** Wait for automatic retry (10–15 days); can't be cancelled
   - **Work not approved:** Confirm work was submitted and reviewed; unapproved hours pay next week
   - **First payout hold:** Confirm it's within 7 days; this is mandatory from Stripe
4. **Verify resolution:** Have them check Stripe dashboard again after fix is applied
5. **Escalate if unresolved:** Direct to support@afterquery.com with full name, login email, payout date, and bank account country

### Helping a contributor troubleshoot a platform bug
1. **Try quick fixes first:** Walk through the troubleshooting list in order (hard refresh, clear cache, incognito, VPN off, desktop)
2. **Gather bug details:** If still broken, collect:
   - Exact page URL where it happened
   - Device and browser (e.g., "Windows 11, Chrome 120")
   - Steps to reproduce (numbered list)
   - Date, time, and timezone
   - Screenshot or error message
3. **Use the bug report template:** Provide the template from report-a-bug page; have them fill it in completely
4. **Submit to support:** Direct them to email the report to support@afterquery.com (or security@afterquery.com if it's a security issue)
5. **Set expectations:** Well-documented reports get fixed faster; security bugs earn bounties ($100–$1,000)

## Common gotchas

- **Onboarding name mismatch:** Account name must match government ID exactly, including middle names. Mismatches cause Persona verification to fail. Have them update their account name before retrying.
- **Stripe country is permanent:** Choosing the wrong country during payment setup can't be undone. If they pick wrong, they must create a new Stripe account. Emphasize this before they continue.
- **VPN breaks verification:** Identity verification and payment setup fail when a VPN is active because it makes location look different. Always have them turn off VPN before starting onboarding.
- **First payout 7-day hold is mandatory:** Stripe requires this; AfterQuery can't override it. Set expectations that the first payout takes longer than subsequent ones.
- **Approved hours vs. logged hours:** Payments are based on approved work, not just logged hours. Unapproved work shifts to the next week's payout. Clarify this when they ask why a payout is lower than expected.
- **Bank account country must match profile location:** Mismatches trigger manual review and delays. Always verify both are the same country before they finish Stripe setup.
- **Assessments can't be retaken:** Contributors get one attempt at each expert pool assessment. Emphasize they should submit with the same care as real project work.
- **Task acceptance is a commitment:** Once accepted, tasks have deadlines. Declining is fine, but accepting and not completing damages reputation. Clarify before they accept.
- **Quality feedback is cumulative:** Low accuracy or inconsistency across multiple tasks can reduce task assignment and priority access. Encourage them to ask for clarification on guidelines early.
- **Email filtering:** Payout notices, project invites, and login emails come from @afterquery.com. If they're not seeing them, check spam folder and add to contacts.

## Verification checklist

Before closing out a support interaction, verify:

- [ ] **Onboarding:** All four steps completed in order; contributor can log in and see dashboard
- [ ] **Payment setup:** Stripe account created with correct business type and country; bank account in same country as profile location
- [ ] **Work guidelines:** Contributor understands the quality checklist and can articulate the core principle (accuracy > speed, consistency matters)
- [ ] **Bug report:** If submitting a bug, all six required fields are included (URL, email, device/browser, steps to reproduce, time, screenshot/error)
- [ ] **Payment issue:** Root cause identified and fix applied; contributor knows what to expect next (e.g., "wait 10–15 days for retry" or "payout comes next Friday")
- [ ] **Troubleshooting:** Quick fixes attempted in order before escalating to support

## Resources

**Comprehensive navigation:** https://docs.afterquery.com/llms.txt — Full page-by-page listing for agent reference

**Critical documentation pages:**
1. [Work Guidelines](https://docs.afterquery.com/articles/about/work-guidelines) — Quality standards, annotation principles, self-review checklist
2. [Contract Work Details](https://docs.afterquery.com/articles/about/contract-work) — Task assignment, payment structure, rights and responsibilities
3. [Payments](https://docs.afterquery.com/articles/payments-taxes/payment-setup) — Payment schedule, Stripe setup, payout estimator, common payment questions

---

> For additional documentation and navigation, see: https://docs.afterquery.com/llms.txt