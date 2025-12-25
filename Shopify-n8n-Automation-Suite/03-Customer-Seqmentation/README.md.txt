# 🎯 Module 03: Marketing & VIP Customer Segmentation

### 🔍 Overview
This system acts as a "Marketing Intelligence" layer. It automatically identifies the purchase behavior of customers in real-time as orders are placed, ensuring that high-value customers are flagged for personalized treatment.

### 🛠️ Business Logic
- **Full Profile Fetch:** Uses the Shopify API to pull deep customer data that isn't provided in the standard order notification.
- **LTV Evaluation:** A logic node calculates the Lifetime Value (LTV) of the customer.
- **Automated Categorization:** - **VIP-LTV:** Applied to top-tier spenders.
    - **LOYAL/NEW/STANDARD:** Applied based on historical purchase frequency.

### 💰 Business Value (ROI)
- **Precision Marketing:** Allows the merchant to create specific email flows for "VIP-LTV" tagged customers.
- **Customer Retention:** Helps the support team prioritize orders from "LOYAL" customers during busy periods.
- **Zero Manual Effort:** Replaces the need for a marketing assistant to manually export and tag customer lists every week.

### 🚀 Technical Setup
1. **Trigger:** Shopify 'On Order Created' Webhook.
2. **API Node:** GET request to fetch the complete Customer Profile.
3. **Logic Node:** Conditional routing based on the LTV variable.
4. **Action:** Shopify 'Tag Order' update node.