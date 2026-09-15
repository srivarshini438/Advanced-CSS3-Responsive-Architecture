# Advanced CSS3 & Responsive Architecture

## 📌 Project Overview

This project is a responsive multi-page portfolio website created using **HTML5, CSS3, and JavaScript**.

The main goal of this project is to demonstrate modern CSS techniques such as **CSS Grid, Flexbox, mobile-first responsive design, CSS variables, and light/dark theme switching**.

The website contains four pages:

* Home
* About
* Projects
* Contact

---

## 🎯 Objectives

The project was developed to:

* Create a responsive website for mobile, tablet, and desktop screens.
* Use **CSS Grid** for two-dimensional layouts.
* Use **Flexbox** for navigation and component alignment.
* Implement a **mobile-first design approach**.
* Use **CSS custom variables** for theme colors.
* Implement a **dynamic Light/Dark Mode** using JavaScript.
* Maintain accessible and semantic HTML5 structure.
* Provide keyboard-friendly navigation and visible focus states.

---

## 🛠️ Technologies Used

* **HTML5** – Semantic structure and webpage content
* **CSS3** – Styling, Grid, Flexbox, media queries, and CSS variables
* **JavaScript** – Light/Dark theme toggle
* **Responsive Design** – Mobile, tablet, and desktop layouts

---

## 📁 Project Structure

```text
Portfolio/
│
├── index.html
├── about.html
├── projects.html
├── contact.html
├── style.css
├── script.js
└── README.md
```

### File Description

| File            | Description                                 |
| --------------- | ------------------------------------------- |
| `index.html`    | Home page of the portfolio                  |
| `about.html`    | Education and technical skills              |
| `projects.html` | Displays portfolio projects                 |
| `contact.html`  | Accessible contact form                     |
| `style.css`     | Main stylesheet and responsive architecture |
| `script.js`     | Light/Dark theme toggle functionality       |
| `README.md`     | Project documentation                       |

---

## 🎨 CSS Features

### 1. CSS Grid

CSS Grid is used for creating two-dimensional layouts, especially for project cards.

Example:

```css
section:has(article) {
    display: grid;
    grid-template-columns: 1fr;
    gap: 20px;
}
```

On larger screens, the layout changes into multiple columns.

```css
@media (min-width: 600px) {
    section:has(article) {
        grid-template-columns: repeat(2, 1fr);
    }
}
```

---

### 2. Flexbox

Flexbox is used for the navigation layout and alignment of navigation components.

```css
nav {
    display: flex;
    flex-direction: column;
    gap: 15px;
}
```

On larger screens:

```css
@media (min-width: 600px) {
    nav {
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
    }
}
```

---

### 3. Mobile-First Responsive Design

The website is designed for smaller screens first.

The default CSS styles target mobile devices, and media queries are then used to adapt the layout for tablets and desktops.

```css
@media (min-width: 600px) {
    /* Tablet styles */
}

@media (min-width: 900px) {
    /* Desktop styles */
}
```

This allows the website to adapt to different screen sizes.

---

## 🌗 Light/Dark Mode

CSS custom properties are used to create the theme system.

### Light Theme

```css
:root {
    --bg-color: #ffffff;
    --text-color: #222222;
    --primary-color: #6c63ff;
}
```

### Dark Theme

```css
body.dark-mode {
    --bg-color: #121212;
    --text-color: #f5f5f5;
    --primary-color: #9b8cff;
}
```

JavaScript adds or removes the `dark-mode` class when the theme button is clicked.

```javascript
const button = document.getElementById("theme-toggle");

button.addEventListener("click", function () {
    document.body.classList.toggle("dark-mode");
});
```

---

## ♿ Accessibility

Accessibility has been considered throughout the project.

The website includes:

* Semantic HTML5 elements
* Proper heading hierarchy
* Navigation labels
* `aria-current` for the active page
* Labels for form inputs
* Required form fields
* Keyboard-friendly navigation
* Visible focus indicators
* Responsive layouts
* Reduced-motion support

Example:

```html
<nav aria-label="Main navigation">
```

---

## 📱 Responsive Breakpoints

The website uses the following breakpoints:

| Screen Size     | Layout  |
| --------------- | ------- |
| Below 600px     | Mobile  |
| 600px and above | Tablet  |
| 900px and above | Desktop |

The layout, navigation, typography, spacing, and project cards adjust according to the screen size.

---

## 🚀 How to Run the Project

1. Download or clone the project.
2. Open the project folder.
3. Make sure all HTML, CSS, and JavaScript files are in the same folder.
4. Open `index.html` in a web browser.
5. Use the navigation menu to move between pages.
6. Click the **Dark Mode** button to switch between light and dark themes.

---

## ✅ Project Requirements Completed

* [x] CSS Grid for two-dimensional layouts
* [x] Flexbox for component alignment
* [x] Mobile-first responsive design
* [x] Responsive media queries
* [x] CSS custom properties
* [x] Light/Dark theme
* [x] JavaScript theme toggle
* [x] Responsive navigation
* [x] Semantic HTML5
* [x] Accessibility features
* [x] Keyboard-friendly form
* [x] Multi-page portfolio structure

---

## 📌 Conclusion

This project demonstrates the use of modern **CSS3 layout and responsive design techniques** to create a flexible and accessible portfolio website.

The combination of **CSS Grid, Flexbox, media queries, CSS variables, and JavaScript** allows the website to provide a consistent experience across mobile, tablet, and desktop devices while supporting both light and dark themes.

---

## 👩‍💻 Author

**Sri Varshini**

BCA Data Science Student

Web Development Intern
