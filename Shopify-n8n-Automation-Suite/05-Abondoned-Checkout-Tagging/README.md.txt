# 🛒 Module 05: Abandoned Checkout Recovery Tagging

### 🔍 Overview
A high-impact marketing automation that tracks lost sales opportunities. This workflow monitors abandoned checkouts in real-time and tags the customer profile, allowing for high-precision recovery campaigns.

### 🛠️ Business Logic
- **Loss Monitoring:** Triggered specifically when a customer exits the checkout flow without completing payment.
- **Data Capture:** Extracts the customer's contact info and the specific products they left behind.
- **System Tagging:** Automatically applies an `ABANDONED-CHECKOUT` tag to the customer resource in Shopify.

### 💰 Business Value (ROI)
- **Revenue Recovery:** Provides the data needed to send automated SMS or email reminders, typically recovering 10-15% of lost carts.
- **Audience Segmentation:** Allows merchants to build a "Hot Leads" list in Shopify for special discount offers.
- **Conversion Insights:** Helps identify if specific products have a high abandonment rate due to price or shipping costs.

### 🚀 Technical Setup
1. **Trigger:** Shopify 'Abandoned Checkout' Webhook.
2. **Logic:** Verification of customer email/phone availability.
3. **Action:** Update Customer/Checkout Tags via Shopify API.