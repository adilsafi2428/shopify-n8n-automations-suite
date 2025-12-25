# 🎖️ Module 08: VIP Customer Alert & Multi-Branch Tagging

### 🔍 Overview
This is a high-level customer intelligence workflow featuring a professional "V-shape" structure. It ensures that high-value orders are not only tagged in the database but also escalated to the management team for immediate attention.

### 🛠️ Business Logic
- **Full Profile Enrichment:** Fetches the complete customer history via the Shopify API to go beyond basic order data.
- **Segment Preparation:** Cleanses and prepares the data for logic evaluation.
- **The "Branching Brain":** A rule-based engine that splits the workflow into three distinct paths:
    1. **Loyalist Path:** Automatically updates Shopify Tags to keep the CRM organized.
    2. **Big Spender Path:** Triggers a high-priority "Gold Alert" via Gmail for immediate sales team notification.
    3. **Frequent Path:** Reserved for future expansion (logging or secondary rewards).

### 💰 Business Value (ROI)
- **High-Touch Service:** Allows store owners to personally thank "Big Spenders" within minutes of a purchase, significantly increasing customer retention.
- **Automated CRM Hygiene:** Eliminates the manual work of identifying and tagging loyal customers.
- **Operational Scalability:** Processes thousands of orders and only alerts humans when a "VIP" event occurs.

### 🚀 Technical Setup
1. **Trigger:** Shopify 'On New Order'.
2. **Data Fetch:** HTTP Request for Full Customer Profile.
3. **Branching:** Switch Node using "Rules" mode for Loyalist/Big Spender/Frequent criteria.
4. **Outbound:** Shopify Tagging + Gmail SMTP "Gold Alert."