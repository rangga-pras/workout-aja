# WorkoutAja - Landing Page Banner Website

This project is a landing page banner created as part of a beginner-level exploration in web development. The goal was to replicate a clean and attractive promotional banner for a fictional workout brand named **WorkoutAja**, while also experimenting with basic styling, layout, and animation using HTML and CSS.

---

## 🔍 Project Overview

The website features:
- A responsive navigation bar with a logo and three menu links.
- A central hero section with text content and a call-to-action button.
- An illustration on the right side.
- A footer with contact information.
- Decorative background elements for visual enhancement.

---

## 🧠 Code Explanation

### 📄 HTML
The HTML structure consists of three main parts:
1. **`<nav>`**: Contains the logo and navigation links.
2. **`<main>`**: The main banner content with a title, description, call-to-action button, and illustration.
3. **`<footer>`**: A small footer with an email link.

Images such as logos and icons are stored in the `images/` folder and referenced from there.

### 🎨 CSS Styling
The CSS is designed to:
- Center the content with `flexbox`.
- Add custom fonts via Google Fonts.
- Apply a linear gradient background for depth.
- Add animations for interactivity.

#### Key Styling Highlights:

- **Global Reset and Font**:
  ```css
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: 'Open Sans', sans-serif;
    background: linear-gradient(...);
  }
  ```
  This ensures consistent spacing and typography across browsers.

- **Navbar Underline Hover Effect**:
  ```css
  nav ul li a::after {
    content: "";
    position: absolute;
    width: 0%;
    height: 2px;
    background-color: #4ECBBD;
    transition: 0.3s;
  }
  nav ul li a:hover::after {
    width: 100%;
  }
  ```
  This adds a smooth underline animation to each nav link on hover.

- **Call-to-Action Button**:
  ```css
  .text button {
    background: #4ECBBD;
    color: #fff;
    padding: 14px 24px;
    border-radius: 6px;
    display: flex;
    align-items: center;
  }

  .text button:hover {
    background: #3EB9A6;
  }
  ```
  This styles the button with brand colors and hover transitions.

- **Layout Responsiveness**:
  The layout uses `flex` and `vw/vh` units to ensure it fits well on most laptop screens.

- **Subtle Animations**:
  Animations using `@keyframes` `floatin` and the `slide in` class (for custom entrance effects) were added for visual appeal. Example:
  ```css
  .slide-in {
  animation: slideIn 1.2s ease-out forwards;
  opacity: 0;
  }
  
  .float-in {
    animation: floatIn 1.4s ease-out forwards;
    opacity: 0;
  }
  
  @keyframes slideIn {
    from {
      transform: translateX(-40px);
      opacity: 0;
    }
    to {
      transform: translateX(0);
      opacity: 1;
    }
  }
  
  @keyframes floatIn {
    from {
      transform: translateY(20px);
      opacity: 0;
    }
    to {
      transform: translateY(0);
      opacity: 1;
    }
  }
  ```

---

## 💡 Summary
This project helped reinforce fundamental HTML/CSS skills such as layout, font integration, hover effects, and subtle animations. It also served as a creative challenge to match a UI design accurately and responsively.

