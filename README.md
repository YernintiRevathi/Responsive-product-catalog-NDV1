# Responsive Product Catalog Page

This project is a single-page static website designed to showcase a product catalog. It is built exclusively with HTML and CSS to demonstrate fundamental web development skills. The layout is fully responsive, adapting seamlessly from large desktop screens to mobile devices using modern CSS techniques like Grid and Flexbox.

---

### **Project Structure**

The project is organized with a clear and simple file structure:
/your-project-folder
│

├── images/

│ ├── product1.webp

│ └── (other product images...)

│

├── index.html # The HTML file containing all the content and structure.

└── style.css # The CSS file containing all visual styles.



---

### **Technologies and Concepts Explained**

This project was built using the following web technologies and concepts, all visible within the provided files.

#### **`index.html` - The Structure**

*   **Header and Navigation (`<header>`, `<nav>`)**: The top of the page contains a `<header>` with a `<nav>` element for the main navigation menu.
*   **Section-Based Layout (`<section>`)**: The page content is divided into logical parts using `<section>` tags. Each section is given a unique `id` (e.g., `#home`, `#products`) which allows the navigation links (`<a href="#products">`) to jump the user to the corresponding section on the same page.
*   **Product Display (`.product-grid`, `.product-card`)**:
    *   The products are organized within a `<div>` with the class `.product-grid`.
    *   Each item is contained in its own `<div>` with the class `.product-card`, which holds the product's image (`<img>`), name (`<h3>`), price, description, and category (`<p>`).
*   **Footer (`<footer>`)**: The page ends with a `<footer>` that includes social media links and copyright information, providing a clean and professional finish.

#### **`style.css` - The Styling and Responsiveness**

*   **CSS Reset (`*`)**: The stylesheet begins with a universal selector `*` to apply `margin: 0`, `padding: 0`, and `box-sizing: border-box`. This creates a consistent baseline across all browsers and makes sizing elements more predictable.
*   **Flexbox for Navigation (`display: flex`)**:
    *   The `.navbar` class uses `display: flex` with `justify-content: space-between` to position the logo/brand on one side and the navigation links on the other.
    *   The social media links in the footer also use `display: flex` to align them neatly in a row.
*   **CSS Grid for the Product Layout (`display: grid`)**:
    *   The `.product-grid` class uses `display: grid` to create the responsive catalog layout.
    *   The line `grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));` is the core of its responsiveness:
        *   `repeat(auto-fit, ...)`: This tells the grid to automatically fit as many columns as it can into the available space.
        *   `minmax(250px, 1fr)`: This defines the size of each column. Each column will have a minimum width of `250px` but can grow to fill an equal fraction (`1fr`) of the remaining space. When there isn't enough space for another 250px column, items wrap to the next line.
*   **Responsive Design with Media Queries (`@media`)**:
    *   A media query, `@media (max-width: 768px)`, is used to apply specific styles for screens that are 768 pixels wide or smaller (like tablets and mobile phones).
    *   Inside this query, the `.navbar` and `.nav-links` have their `flex-direction` changed to `column`. This stacks the navigation links vertically, making them easy to use on a narrow screen.

---

### **How to Run This Project Locally**

This project does not require any installation or special tools.

1.  **Download or Clone the Files**: Make sure you have the `index.html` file, the `style.css` file, and the `images` folder all together in one main project folder.
2.  **Open the HTML File**: Navigate to the project folder on your computer and double-click the `index.html` file.
3.  **View in Browser**: The file will automatically open in your default web browser, and the website will be displayed. You can resize the browser window to see the responsive design in action.
 
with 💗 by **Revathi**
