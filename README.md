# Automail - Your Smart Email Assistant 💌

Welcome to **Automail**!  
Automail is a smart and flexible Email Assistant built to automate your email responses and actions. It helps you manage emails with ease, making your workflow faster, more efficient, and fully customizable. ✨  

👉 Explore the *[Use Cases](./examples/usecases.md)* to see Automail in action!  

---

## Features 🌟
- Send automatic out-of-office (OOO) replies  
- Forward emails to specified addresses  
- Reply with custom templates  
- Trigger HTTP requests based on incoming emails  
- Log email activity to files  
- Save email content or custom text locally  
- Use placeholders to insert dynamic values in templates  

---

## Supported Email Actions ✉️
- [x] `email` - Send a new email  
- [x] `reply_email` - Reply to an existing email  
- [x] `forward_email` - Forward an email  
- [x] `HTTPRequest` - Perform an HTTP GET or POST request  
- [x] `log` - Save log data to a file  
- [x] `saveToFile` - Write text or email content to a file  

---

## Placeholders 📝
Automail allows you to use placeholders in your templates to dynamically insert information:  

- `{name}` → Sender’s name  
- `{email}` → Sender’s email address  
- `{subject}` → Email subject  
- `{body}` → Email body  
- `{emailDate}` → Date the email was received  
- `{date}` → Today’s date (YYYY-MM-DD)  
- `{date_day}` → Current day number (e.g., 12)  
- `{date_month}` → Current month (e.g., 3)  
- `{date_year}` → Current year (e.g., 2023)  
- `{date_weekday}` → Current weekday (e.g., Monday)  
- `{date_weekday_short}` → Current weekday short form (e.g., Mon)  

---

## Placeholder Logic 🧠
Automail also supports conditional logic with placeholders to create smarter actions:  

- `= "VALUE"` → Matches exact values  
  - Example: `{email = "example@abc.com"}`  
  - Must end with `{end}`  

- `contains "VALUE"` → Matches partial values  
  - Example: `{email contains "example"}`  
  - Must end with `{end}`  

---
