# AutoSecure – Guidewire PolicyCenter Showcase

This is a self-initiated mini project that simulates a real-world configuration scenario in Guidewire PolicyCenter. The purpose of this showcase is to demonstrate hands-on understanding of core PolicyCenter components such as product modeling, PCF customization, rule configuration, and system integration.

## 📘 Project Summary

**Business Case:**  
AutoSecure is a fictional insurance company offering Personal Auto Insurance. As a PolicyCenter Configuration Developer, I designed and configured a basic product setup including policy components, screen customization, underwriting rules, and mock REST integration.

---

## 🛠️ Key Features Implemented

### 1. Product Model Design
- Personal Auto Product with coverages like Liability, Collision, and Comprehensive
- Question sets for driver and vehicle details
- Availability conditions based on driver profile

### 2. PCF Customization
- Custom `AccountSummary.pcf` screen with:
  - Recently issued policies section
  - Customer preferred contact method field
  -  “Customized AccountSummary.pcf to add recent policies and preferred contact info”

### 3. Underwriting Rules
- Reject policy if driver age is under 18
- Require manual approval if vehicle value > ₹20,00,000

### 4. Integration (Mock)
- REST API mock to fetch driver's accident history
- Sample request/response in JSON format

---

## 📂 Project Structure

