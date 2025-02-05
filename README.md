# Job Application Form

This is a simple yet functional **job application form** built using HTML. It provides a structured way for applicants to submit their **personal and employment details** along with their **resume**. The form follows a clean layout and ensures that necessary fields are filled before submission.

## Features
- Collects personal details such as **name, email, phone number, and address**.
- Includes fields for **employment-related information** like the position applied for, LinkedIn profile, and personal website/portfolio.
- Allows applicants to **upload their resume** in PDF, DOC, or DOCX formats.
- Uses **`<fieldset>`** and **`<legend>`** tags for better organization and readability.

## File Structure
```
/job-application-form
│── index.html   # Contains the full structure of the job application form.
│── index.css    # Contains the complete CSS of the application.
```

## Code Explanation

Below are descriptions of a few sections that might be harder to understand:

### 1. `<fieldset>` and `<legend>` for Grouping Form Sections  
The `<fieldset>` tag is used to **group related fields** together, making the form more structured.  
The `<legend>` tag provides a **title for the grouped section**.

#### Example:
```html
<fieldset>
    <legend>Personal Information</legend>
    <label for="fname">First Name:</label><br>
    <input type="text" id="fname" name="fname" required><br><br>
</fieldset>
```
✔ **Why is this important?**  
It visually and semantically **separates form sections**, making it easier for users to understand.

---

### 2. `<input type="file">` for Resume Upload  
This input field allows users to **upload files** (PDF, DOC, DOCX only).

#### Example:
```html
<input type="file" id="resume" name="resume" accept=".pdf, .doc, .docx" required>
```
✔ **Key Attribute:**  
`accept=".pdf, .doc, .docx"` → Restricts file types to resumes only.

---

### 3. `required` Attribute for Mandatory Fields  
Ensures that users **fill in important fields** before submitting.

#### Example:
```html
<input type="email" id="email" name="email" required>
```
✔ **Why?**  
The `required` attribute ensures users **cannot submit the form without filling in the field**.

---

## Future Improvements
- 📌 **Adding CSS** for better styling and user experience.
- 📌 **Implementing JavaScript validation** to enhance form validation before submission.
- 📌 **Integrating a backend** (e.g., PHP, Node.js) to process and store submitted applications.

## 📜 License  
This project is **open-source** and free to use.

✅ **Happy Coding!** 🚀

