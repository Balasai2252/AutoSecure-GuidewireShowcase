# 🗂️ Batch Job: Unconverted Quote Reminder

**Batch Name:** `UnconvertedQuoteReminderBatch`  
**Frequency:** Daily at 2 AM  
**System:** Guidewire PolicyCenter (simulated)

---

## 📝 Purpose

Automatically identify and notify customers whose quotes are older than 10 days and not yet converted into policies.

---

## 🔍 Criteria

- `QuoteDate < today - 10`
- `QuoteStatus = 'Quoted'`
- `IsConverted = false`

---

## ⚙️ Actions Performed

- Sends an email reminder to the customer/agent
- Adds a note to the quote activity log

---

## 🧪 Testing Considerations

- Run with test data: one recent quote, one old quote
- Verify activity notes and dummy notification log

---

*Note: This is a mock batch configuration for portfolio/demo use only.*
