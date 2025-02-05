# Daily News Blog

This is a simple and responsive news blog built using **HTML** and **CSS**. It features a structured layout with sections for breaking news, technology, and health articles. The blog incorporates text, images, audio, and video elements, making it an engaging platform for delivering news content.

## Features
✅ **Responsive Design** – Ensures a smooth viewing experience on different devices.  
✅ **Navigation Bar** – Provides easy access to different sections of the blog.  
✅ **News Articles** – Includes multiple articles with text, images, and embedded media (**audio & video**).  
✅ **Styled with CSS** – The blog uses modern CSS techniques to enhance readability and design.

## File Structure
```
/daily-news-blog
   ├── index.html   → The main HTML file containing the structure of the news blog.
   ├── index.css    → The CSS file that styles the blog layout.
   ├── assets/      → Folder for storing images, audio, and video files.
       ├── images/  → Contains images used in the blog.
       ├── audio/   → Stores the news audio files.
       ├── video/   → Stores embedded video files.
```

## Code Explanation

### 1. `<fieldset>` and `<legend>` in Forms
```html
<fieldset>
    <legend>Personal Information</legend>
    <label for="fname">First Name:</label><br>
    <input type="text" id="fname" name="fname" required><br><br>
</fieldset>
```
✔ **Explanation:**
- `<fieldset>` groups related form elements together for better structure and accessibility.
- `<legend>` provides a title for the group of fields, improving readability.

📌 **Why it's useful?**
It enhances form usability and makes it visually clearer when multiple sections are present.

---

### 2. `<source>` Inside `<audio>` and `<video>`
```html
<audio controls>
    <source src="assets/audio/news-audio1.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>
```
✔ **Explanation:**
- `<source>` inside `<audio>` or `<video>` allows multiple formats to be specified.
- The browser picks the best-supported format automatically.
- The fallback text *"Your browser does not support the audio element"* appears if no format is supported.

📌 **Why it's useful?**
Some browsers may not support specific audio or video formats. Using multiple `<source>` tags ensures compatibility.

---

### 3. `<video>` Embedding (Issue in Your Code)
```html
<video controls>
    <source src="https://www.youtube.com/shorts/KgzmJUUk8w0?feature=share" type="video/mp4">
</video>
```
🚨 **Why isn't this working?**
- YouTube **does not allow direct embedding** of its videos via `<video>` and `<source>`.
- Instead, use an `<iframe>` like this:
```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/KgzmJUUk8w0" frameborder="0" allowfullscreen></iframe>
```
📌 **Why it's useful?**
If you need to embed **YouTube videos**, `<iframe>` is the correct method.

---

### 4. `<meta name="viewport">`
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
✔ **Explanation:**
- This tag **controls how the website scales** on mobile devices.
- `width=device-width` ensures the page **matches the screen width**.
- `initial-scale=1.0` ensures the page **is not zoomed in or out** by default.

📌 **Why it's useful?**
Without this, websites can appear **too zoomed-in or too small** on mobile devices.

---

## Future Improvements
🚀 Adding **CSS animations** for better user engagement.  
🚀 Implementing **JavaScript validation** to enhance form validation before submission.  
🚀 Integrating a **backend (e.g., PHP, Node.js)** to process and store submitted articles.

## Author
**Your Name**  
📧 [arpita.sinha@pw.live](mailto:YourEmail@example.com)  
🔗 [GitHub Profile](https://github.com/YourGitHubArpitaSinha02)

---


