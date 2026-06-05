# AI Food Ordering Assistant using n8n, Google Gemini & Google Sheets

## Project Overview

This project is an AI-powered Food Ordering Assistant built using n8n, Google Gemini, and Google Sheets.

The assistant allows customers to:

- View available menu items
- Place food orders
- Check stock availability
- Get FAQ information
- Store confirmed orders automatically

The system uses Google Sheets as a lightweight database and Google Gemini as the conversational AI model.

---

## Technologies Used

- n8n
- Google Gemini API
- Google Sheets
- AI Agent
- Simple Memory

---

## Workflow Architecture

User Chat
↓
AI Agent
↓
Google Gemini
↓
Google Sheets

- Items Sheet (Inventory)
- FAQ Sheet
- Confirmation Sheet

---

## Features

### Menu Management

The assistant reads food items from the Google Sheets inventory.

Example:

- Chicken Curry
- Butter Chicken
- Mutton Curry
- Prawn Masala
- Crab Curry

### Order Placement

Users can place orders by providing:

- Name
- Food Item
- Quantity

The assistant verifies item availability before confirming the order.

### Inventory Check

The system checks stock from the Items sheet.

Available items:

- Status = Yes

Unavailable items:

- Status = No

### FAQ Support

The assistant answers questions regarding:

- Opening hours
- Delivery availability
- Refund policy
- Vegetarian options
- Payment methods

### Order Storage

Confirmed orders are automatically stored in the Confirmation sheet with:

- Customer Name
- Food Item
- Quantity Ordered
- Order Date
- Status

---

## Google Sheets Structure

### Items Sheet

| Food Item | Quantity | Status |
|------------|-----------|---------|
| Chicken Curry | 35 | Yes |
| Butter Chicken | 28 | Yes |
| Fish Curry | 0 | No |

### Confirmation Sheet

| Customer Name | Food Item | Quantity Ordered | Order Date | Status |
|--------------|-----------|------------------|------------|---------|

### FAQ Sheet

| Question | Answer |
|-----------|---------|

---

## Sample Conversation

User:
Hi

Bot:
Welcome to Supriya Tasty Foods 🍽️

How can I help you today?

🍽️ Place an order
📘 FAQ / Information
📦 Check order / stock

User:
Provide me the list

Bot:
Available Items:

- Chicken Curry
- Butter Chicken
- Mutton Curry
- Crab Curry

User:
Chicken Curry

Bot:
Could you please tell me your name and quantity?

User:
Gowri

User:
2

Bot:
Your order for Chicken Curry (2) is confirmed ✅

---

## Future Enhancements

- WhatsApp Integration
- Payment Gateway Integration
- Order Cancellation Workflow
- Real-time Inventory Updates
- Order Tracking System
- Error Handling Improvements

---

## Screenshots
Ai-Agent-workflow
<img width="1919" height="973" alt="image" src="https://github.com/user-attachments/assets/e530b634-949e-439d-a440-92b93198cc43" />


Filter
<img width="1919" height="966" alt="image" src="https://github.com/user-attachments/assets/9cc297f1-b647-446a-91f8-fa5fae4211d8" />


