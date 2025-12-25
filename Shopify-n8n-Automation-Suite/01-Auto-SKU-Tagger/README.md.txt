# 🏷️ Module 01: Intelligent SKU Auto-Tagging System

### 🔍 Overview
A high-performance automation designed to eliminate manual order sorting. This system monitors incoming Shopify orders and instantly applies specific tags based on SKU patterns.

### 🛠️ Business Logic
- **Pattern Matching:** Scans line items for specific SKU strings (e.g., "DIGITAL-", "FRAGILE-").
- **Dynamic Tagging:** Automatically updates the Shopify Order resource with relevant operational tags.
- **Error Handling:** Designed to bypass orders without matching SKUs to save API resources.

### 💰 Business Value (ROI)
- **Reduces Human Error:** 0% chance of a "Digital" item being sent to a physical warehouse.
- **Saves Labor:** Reclaims ~5-10 hours/month of manual tagging for mid-sized stores.
- **Faster Fulfillment:** Orders are categorized the millisecond they are created, allowing for instant filtering by warehouse staff.

### 🚀 Technical Setup
1. **Trigger:** Shopify 'Order Created' Webhook.
2. **Logic:** IF/Filter nodes for SKU validation.
3. **Action:** Shopify API 'Update Order' via GraphQL/REST.