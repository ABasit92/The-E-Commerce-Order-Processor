# 🛒 E-commerce Order Processor

## 📖 Overview
The **E-commerce Order Processor** is an **n8n workflow** designed to automate the order fulfillment process for online stores.  
It handles **stock validation, packing list generation, and warehouse notifications** – ensuring smooth and efficient operations.

---

## 🚀 Features
- **Webhook Trigger** – Listens for new order data (simulated or real).
- **Inventory Check** – Looks up product stock levels in Google Sheets.
- **Logic & Alerts**:
  - ❌ If items are out of stock → Drafts an email alert to inventory manager.
  - ✅ If items are in stock → Creates a fulfillment record with a **formatted packing list**.
- **Notifications** – Notifies warehouse/fulfillment team via messaging app.

---

## 🖼️ Screenshot
<img width="1354" height="645" alt="1" src="https://github.com/user-attachments/assets/9a184ca1-41e9-4b1b-bf9e-4511e93d5fbd" />

---

## 🛠️ Tech Stack
- [n8n](https://n8n.io/) – Workflow automation
- Webhook – Order data input
- Google Sheets – Inventory database & fulfillment queue
- Email – Stock issue alerts
- Slack/Discord – Team notifications

---

## 📂 Workflow
1. Customer places an order → Order data sent to workflow via Webhook.
2. Items are checked against Google Sheets inventory.
3. Workflow decides:
   - Out of stock → Send email to inventory manager.
   - In stock → Generate fulfillment record & packing list.
4. Notification sent to warehouse team for action.

---

## 🌟 Use Case
Perfect for e-commerce stores that need:
- **Automatic inventory validation**.
- **Instant alerts** for low/out-of-stock issues.
- **Packing list generation** without manual effort.
- **Real-time notifications** for fulfillment teams.


