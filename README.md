# 🥗 Weekly Meal Planner Web App

This is a **static web-based Meal Planner** designed to help users organize their weekly meals with ease. The app provides a clean and printable layout for planning Breakfast, Lunch, Dinner, and Snacks for each day of the week — plus a built-in grocery list section.

🔗 **Live Demo:** [https://afsheenmahmood.github.io/gh-pages-demo/](https://afsheenmahmood.github.io/gh-pages-demo/)

---

## 📌 What This Project Does

This meal planner allows users to:
- Plan meals for **all 7 days** of the week
- Separate meals into **Breakfast, Lunch, Dinner, and Snacks**
- **Mark meals with checkboxes** as planned or completed
- Use a **static grocery list section** to write down ingredients
- **Print** the planner and grocery list for physical use
- Enjoy a clean, mobile-friendly layout made using **CSS Grid**

It’s a perfect tool for:
- Meal prep enthusiasts
- Busy families or individuals
- Diet planning
- Reducing food waste

---

## 🚀 How It Works

### 1. **Layout and Structure**
- The meal planner uses an HTML `<table>`-like layout created using **CSS Grid**.
- Each row represents a day of the week, and each column represents a meal type.
- Inside each grid cell is a meal item with a **custom-styled checkbox**.

### 2. **Checkboxes**
- Users can click checkboxes next to meal names to track what’s planned or done.
- These checkboxes are purely **client-side**, and state is not saved after refresh (but can be extended using localStorage).

### 3. **Grocery List**
- A `<textarea>` element is provided for users to manually type in grocery items.
- The list can be printed along with the meal plan.

### 4. **Print Support**
- The page is printable using your browser’s **Print** feature (`Ctrl + P` or `Cmd + P`).
- You can take a printed copy to the store or hang it on your fridge!

---

## 🖼 Technologies Used

| Technology          | Description                            |
|---------------------|----------------------------------------|
| HTML5               | For basic structure of the website     |
| CSS3                | For styling, layout, and grid system   |
| GitHub Pages        | To host and serve the website          |
| GitHub Actions      | To automate deployment to GitHub Pages |
| peaceiris/actions-gh-pages | GitHub Action used to deploy         |

---


## ⚙️ Deployment (via GitHub Actions)

This project is deployed using [peaceiris/actions-gh-pages](https://github.com/peaceiris/actions-gh-pages), a popular GitHub Action to automate deployment to GitHub Pages.

### How it works:
- You push changes to the `main` branch
- GitHub Actions copies the files from the `src/` folder into a `public/` folder
- The `public/` folder is published to the `gh-pages` branch
- GitHub Pages uses the `gh-pages` branch to serve the site at your username.github.io

### Workflow Highlights:
```yaml
on:
  push:
    branches:
      - main
