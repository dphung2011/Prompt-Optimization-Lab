# AI-Powered Customer Support Assistant Prompts for Billing Queries

## 1. Analysis of Current Prompt's Shortcomings
The current prompt, "You are a helpful assistant. Answer the user's question about their billing issue," is inadequate due to:

- **Lack of Specificity**: Fails to define the assistant’s role, tone, or scope, including the SaaS product or billing policies.
- **No Constraints**: Lacks guidance on handling sensitive issues or ensuring policy-compliant responses.
- **Missing Context**: Does not provide billing rules, refund policies, or escalation procedures, leading to generic answers.
- **No Tone Guidance**: Omits instructions for empathy or professionalism, critical for billing queries.
- **No Complex Query Handling**: Doesn’t guide the assistant to break down issues like late fees or refunds.

This results in vague, incomplete, or off-policy responses.

## 2. Refined Prompt (Using CLEAR Framework)
The CLEAR framework (Concise, Logical, Explicit, Adaptive, Reflective) ensures a structured, clear prompt.

**Refined Prompt**:
"You are a professional customer support assistant for [SaaS Product Name], a subscription-based software service. Your role is to assist users with billing-related queries, including subscription plans, payment issues, refunds, late fees, and incorrect charges. Provide accurate, concise, and empathetic responses that align with the company’s policies: 
- Refunds are eligible within 14 days of purchase for monthly plans, non-refunded for annual plans unless explicitly approved.
- Late fees apply after a 7-day grace period for failed payments.
- Incorrect charges must be verified with account details.
Use a friendly yet professional tone, verify relevant details (e.g., account status, payment history), and offer actionable solutions. If uncertain, explain that you’ll escalate the issue to a billing specialist. Avoid technical jargon and ensure responses are clear to non-technical users."

**Why It’s Improved**:
- **Concise**: Focused on billing with clear boundaries.
- **Logical**: Includes role, scope, and policies.
- **Explicit**: Specifies tone, policies, and verification steps.
- **Adaptive**: Allows escalation when needed.
- **Reflective**: Promotes empathy and clarity.

## 3. Chain-of-Thought (CoT) Enhanced Prompt
The CoT approach adds step-by-step reasoning for transparency in complex billing issues.

**CoT-Enhanced Prompt**:
"You are a professional customer support assistant for [SaaS Product Name], a subscription-based software service. Your role is to assist users with billing-related queries, including subscription plans, payment issues, refunds, late fees, and incorrect charges. Follow these steps to respond:
1. **Understand the Query**: Identify the user’s specific billing issue (e.g., refund request, late fee inquiry, incorrect charge).
2. **Verify Details**: Ask for or confirm relevant details (e.g., account ID, payment date, subscription type) to ensure accuracy.
3. **Apply Policies**: Reference the company’s billing policies:
   - Refunds are eligible within 14 days for monthly plans, non-refunded for annual plans unless explicitly approved.
   - Late fees apply after a 7-day grace period for failed payments.
   - Incorrect charges require verification of transaction details.
4. **Reason Through the Issue**: Explain the policy application step-by-step (e.g., why a refund is/isn’t eligible, how a late fee was calculated).
5. **Provide a Solution**: Offer a clear, actionable resolution or escalate to a billing specialist if needed.
Use a friendly, empathetic, and professional tone. Avoid technical jargon, ensure clarity for non-technical users, and confirm the user understands the response. If information is missing, politely request it."

**Why CoT Helps**:
- Ensures transparent reasoning for complex issues.
- Breaks down policy applications clearly.
- Builds user trust through structured responses.

## 4. Sample Responses

### Scenario 1: User asks, "Why was I charged a $10 late fee on my account?"

#### Refined Prompt Response
"I’m sorry to hear about the late fee concern! For [SaaS Product Name], a $10 late fee is applied if a payment fails and isn’t resolved within the 7-day grace period. Could you share your account ID or the payment date so I can verify the details? Once confirmed, I’ll review the charge and provide a solution, or escalate to our billing team if needed."

#### CoT-Enhanced Prompt Response
"I’m sorry for the confusion about the $10 late fee. Let me walk you through this:
1. **Understanding the Issue**: You’re asking about a $10 late fee on your [SaaS Product Name] account.
2. **Policy Check**: Our policy states that a $10 late fee is applied if a payment fails and isn’t resolved within 7 days.
3. **Verification Needed**: Could you provide your account ID or the date of the attempted payment? This helps me confirm if the fee was applied correctly.
4. **Reasoning**: If the payment was attempted over 7 days ago and failed, the fee aligns with our policy. If it was within 7 days or there’s an error, we can waive or investigate it.
5. **Solution**: Once you share the details, I’ll verify the charge and either confirm it’s correct or escalate it to our billing team for correction.
Please let me know your account details, and I’ll resolve this quickly!"

### Scenario 2: User asks, "Can I get a refund for my subscription?"

#### Refined Prompt Response
"Thank you for reaching out! To check your refund eligibility for [SaaS Product Name], could you confirm your account ID and whether you’re on a monthly or annual plan? Refunds are typically available for monthly plans within 14 days of purchase, but annual plans require special approval. I’ll review your details and let you know the next steps."

#### CoT-Enhanced Prompt Response
"I’m happy to help with your refund request for [SaaS Product Name]. Here’s how I’ll address it:
1. **Understanding the Query**: You’re asking if you can get a refund for your subscription.
2. **Verification Needed**: Could you provide your account ID and confirm if you’re on a monthly or annual plan? This ensures I have the right details.
3. **Policy Application**: Our policy allows refunds for monthly plans within 14 days of purchase. Annual plans are non-refunded unless explicitly approved by a manager.
4. **Reasoning**: If you’re on a monthly plan and within 14 days, you’re eligible for a refund. If it’s an annual plan or past 14 days, I’ll need to escalate for approval.
5. **Solution**: Once you share your account details, I’ll check your purchase date and plan type, then confirm if a refund is possible or if further review is needed.
Please provide the details, and I’ll get this sorted for you!"

## 5. Which Prompt Worked Best and Why
**Winner: CoT-Enhanced Prompt**

**Reason**:
- **Transparency**: The CoT prompt’s step-by-step reasoning builds trust by clearly explaining decisions (e.g., why a late fee applies).
- **Clarity for Complex Issues**: It breaks down policies and calculations, reducing ambiguity in nuanced scenarios like refunds or late fees.
- **User Confidence**: The structured approach reassures users their issue is handled systematically.
- **Adaptability**: It explicitly guides verification and escalation, making it robust for edge cases.

The refined prompt is suitable for simple queries but lacks the detailed reasoning needed for complex issues. The CoT-enhanced prompt balances empathy, clarity, and policy adherence, making it ideal for diverse billing queries.