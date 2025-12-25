# 📉 Module 04: Inventory Low-Stock Alert System

### 🔍 Overview
A critical logistics automation that monitors stock levels in real-time. This system ensures that the merchant is notified the moment a product's inventory drops below a safe threshold, preventing "Out of Stock" scenarios.

### 🛠️ Business Logic
- **Inventory Monitoring:** Triggered by every successful order.
- **Real-time Quantity Check:** Queries the Shopify `inventory_level` API for the specific SKU/Location ID.
- **Threshold Logic:** An IF Node checks if `available_quantity <= 5` (Customizable).
- **Instant Alert:** Routes a high-priority notification to the management team.

### 💰 Business Value (ROI)
- **Protects Revenue:** Ensures products are restocked before they sell out, maintaining constant sales flow.
- **Ad Spend Efficiency:** Prevents wasting marketing budget on ads for items that cannot be purchased.
- **Automated Auditing:** Replaces the need for staff to manually check inventory levels every morning.

### 🚀 Technical Setup
1. **Trigger:** Shopify 'Order Created' (or 'Inventory Level Updated').
2. **API Node:** Fetching available quantity from Shopify Inventory API.
3. **Logic Node:** Threshold evaluation (e.g., Alert if < 5 units).
4. **Action:** Email/Slack notification to the Warehouse Manager.