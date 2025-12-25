# 🛡️ Module 02: Real-time Fraud & Risk Mitigation

### 🔍 Overview
An automated security layer that analyzes the "Risk Level" of every incoming Shopify order. This system acts as a firewall, preventing the fulfillment of suspicious transactions.

### 🛠️ Business Logic
- **Risk Analysis:** Queries the Shopify Order Risk API.
- **Decision Engine:** Evaluates risk scores (Low, Medium, High).
- **Security Action:** If 'High Risk' is detected, the system applies a "FRAUD-CHECK" tag and halts any auto-fulfillment processes.

### 💰 Business Value (ROI)
- **Prevents Chargebacks:** Saves the merchant from losing both the product cost and the transaction value.
- **Protects Merchant Standing:** Keeps the store's "Chargeback Ratio" low, preventing payment gateway bans.
- **Operational Safety:** Alerts the manager via email/system-tag for manual review.

### 🚀 Technical Setup
1. **Trigger:** Shopify 'Order Created' Webhook.
2. **Logic:** HTTP Request to `/orders/{order_id}/risks.json`.
3. **Action:** Conditional branching based on the `recommendation` field.