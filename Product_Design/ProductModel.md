# 📦 Personal Auto Insurance Product Model – AutoSecure

This document outlines the product model configuration for the **Personal Auto Insurance** product, created as part of the AutoSecure Guidewire PolicyCenter showcase project.

---

## 🧾 Product Details

- **Product Name:** Personal Auto Insurance  
- **Policy Line:** PersonalAutoLine  
- **Description:** Insurance coverage for individually owned private vehicles.

---

## 🧩 Product Model Table

| Section        | Element Name                | Type         | Description / Condition                            |
|----------------|-----------------------------|--------------|----------------------------------------------------|
| Product        | Personal Auto Insurance      | Product      | Insurance product for privately owned vehicles     |
| Policy Line    | PersonalAutoLine             | Policy Line  | Line containing all coverages for vehicle policy   |
| Coverage       | LiabilityCoverage            | Coverage     | Covers third-party damage                          |
| Coverage       | CollisionCoverage            | Coverage     | Covers vehicle collision damage                    |
| Coverage       | ComprehensiveCoverage        | Coverage     | Covers theft, fire, weather damage                 |
| Question Set   | DriverQuestionSet            | Question Set | Captures driver's age, history, license details    |
| Question Set   | VehicleQuestionSet           | Question Set | Captures vehicle model, make, year, and value      |
| Availability   | Driver Age > 18              | Condition    | Show coverages only if driver is over 18           |
| Availability   | Vehicle Value < ₹20 Lakhs     | Condition    | For direct issue, else goes to underwriting review |

---

## 📌 Assumptions

- The product is designed for the Indian market with INR currency.
- Coverage selection and availability depend on simple rule-based criteria.
- This model simulates only high-level components for demonstration purposes.

