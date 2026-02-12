# My-learning-process

For this workshop project, I chose to combine two things I truly enjoy: building websites and cooking (and of course, enjoying the food as well).
With this website, I want to showcase some of my cooking skills while practicing and demonstrating my HTML and CSS knowledge. This project allows me to be creative both in the kitchen and in front of the computer.

The original workshop instructions are included below this report. I used them as a guideline and followed each step carefully while developing the project.

---

### Step 1 – Create the header

I added a '<header>' to my homepage to welcome visitors and provide structure.

- The header now does not contain text directly, but instead displays a background image with the bottom part visible, showing my "Coocking Adventures with Kristy" banner. I wanted to write some text there first, but it didn't look right with the background-image. 
- I used CSS background-image to set the header image, background-size: cover to fill the header, and background-position: bottom center to ensure the important part of the image (the bottom) remains visible even on larger screens. 
- A <nav> element is placed at the bottom of the header, styled with position: absolut; bottom: 0; left:0; widht: 100% to span the full widht. The links are centred using Flexbox. 

**Note on debugging the navbar:**
Initially, the navbar appeared only on the righ side of the header. I tried several approaches, including adjusting widhts and flex settings, but the issue persisted. Eventually, I realized that adding left: 0; to the CSS positioning fixed it and ensured the navbar spanned the full widht as intended. This taught me a lot about absolute positioning and how it interacts with parent elements and flex layouts.  

- Using CSS instead of <img> for the header background allows more flexibility for positioning and ensures the header scales well on diffrent screen sizes. 


---

## Step 2 – Create the main content

I added a `<main>` section below the header to display the primary content of the page:

- `<h1>` contains: "Welcome to my website!"  
- `<p>` contains a short description: "Discover my favorite recipes and cooking adventures while at the same time following my journey as I learn and grow in HTML and CSS on my path to becoming a full-stack developer."
- The main content is centered and uses padding and text styling for readability.

---

## Step 3 – Footer

I added a `<footer>` at the bottom of the page:

- Contains a simple copyright line: "© 2026 Cooking Adventures with Kristy"
- Styled with a background color and centered text. I will change this later. This is just a start. 

---

## Step 4 – CSS Styling

- **Header:** background image, `cover` size, `bottom center` position, height set to 400px, and `position: relative` for navbar positioning.  
- **Navbar:** absolute position at the bottom of the header, full width, semi-transparent background (`rgba`), links centered using Flexbox.  
- **Main content:** centered text, readable font size, padding applied.  
- **Footer:** full-width, centered text, contrasting background for clarity.

---

## Step 5 – Footer Improvements & Main Content Testing

After initially adding a simple footer, I made several improvements to ensure it looked better and behaved correctly on the page:

- I changed the footer to a **pink background (`#ea4199`)** with **white, centered text** for better visual contrast.  
- Using **flexbox on the body**, I ensured that the footer **always stays at the bottom of the viewport**, even if the main content is short. This removed the unwanted white space that previously appeared below the footer.  
- I added **padding to the footer** (`15px 0`) to give the text some breathing room and improve readability.  
- I added temporary **lorem ipsum text** in the main content to test the layout and spacing of paragraphs.  
- To create consistent spacing between paragraphs, I **removed `<br>` tags** and applied CSS `margin-bottom` to `<p>` elements, which improved readability and ensured a neat, professional look.  

> **Reflection:** Fixing the footer and testing the main content helped me practice **layout control**, **flexbox**, and **page structure**. I also learned the importance of proper semantic HTML (`<p>` tags instead of `<br>` for spacing) and how CSS can be used to manage spacing consistently across the page. These adjustments improved both the **visual design** and **responsiveness** of the webpage.


## Step 6 – Contact Form

I added a **contact form** to the website on `contact.html`:

- The form includes fields for **Name**, **Email Address**, and **Message**.  
- A **submit button** allows users to send their message.  
- The form uses semantic HTML elements (`<form>`, `<label>`, `<input>`, `<textarea>`).  
- Styled with CSS (`.contact-form` class) to match the website’s design: centered, responsive, with padding, background color, and a hover effect on the submit button.  
- This form layout was adapted from a previous assignment for consistency.

## Step 7 – Header and Navbar on All Pages  

I ensured that the **header and navbar are consistent across all pages** (`index.html`, `food.html`, and `contact.html`):

- The `<header>` contains a background image that is always 400px high.  
- A navbar with links to **Home**, **Food**, and **Contact** is positioned at the bottom of the header using `position: absolute; bottom: 0; left: 0; width: 100%;`.  
- Flexbox (`display: flex; flex-direction: column; justify-content: flex-end;`) ensures the navbar stays at the bottom even when the header content is empty.  
- The background image uses `background-size: cover;` and `background-position: bottom center;` so the important part of the image remains visible on all screen sizes.  
- This approach allows the header and navbar to be reused on multiple pages for a consistent layout.

---

## Step 8 – Food Table  

On the `food.html` page, I added a **table layout** to showcase recipes and descriptions:

- Each row contains an image of the dish and a short description beside it.  
- The table uses CSS to remove default borders and keep a clean look (`border-collapse: collapse; border: none;`).  
- Images are styled with a fixed width (150px), rounded corners, and proper spacing.  
- This layout allows users to scan dishes visually while still including descriptive text.  
- The table structure can easily be expanded with additional dishes or adjusted for styling improvements.

** note **
I'm not really happy yet with the style, so I will change this part soon. 

---

## Step 9 – Footer  

The `<footer>` is consistent across all pages:

- Full-width layout with a pink background (`#ea4199`) and centered white text.  
- Positioned at the bottom of the page using Flexbox:  
  - `body { display: flex; flex-direction: column; }`  
  - `main { flex-grow: 1; }`  
- This ensures the footer stays at the bottom even when the page content is short.

---

## Step 10 – General CSS Styling  

General styling improvements were applied across the entire website:

- A CSS reset was added to remove default browser spacing:  
  `* { margin: 0; padding: 0; box-sizing: border-box; }`  
- Consistent fonts, colors, spacing, and layout applied to all pages.  
- Navbar links include hover effects for improved interactivity.  
- The contact form and food table are styled for readability, responsiveness, and visual consistency.

------------------------------------------------------------------------------------------------------------------
![Lexicon Logo](https://lexicongruppen.se/media/wi5hphtd/lexicon-logo.svg)

# Workshop: HTML & CSS

The task is to create a **single webpage** using **HTML** and **CSS**. The page must include:

- A **header**
- A **main** content section
- A **footer**
- At least **one table**
- At least **one form**
- Use **semantic HTML elements** for structure
- Use **CSS selectors** for styling
- **Advanced layout (e.g., Flexbox or Grid) is optional**

Use **semantic HTML elements** to organize the content and **CSS selectors** to style the page in a clear and consistent way.

---

## Project Ideas (choose one)

- A profile page to introduce yourself  
- A café information page presenting menu highlights, hours, and contact  
- A product shipping information page with product details and an order form  
- An event announcement page with schedule and sign-up form  
- A club or group introduction page with a table of members and a contact form  

---

## Project Setup

1. **Create a new GitHub repository**  
   Name it **`html-css-workshop`** or choose a name related to your idea.

2. **Add your project files**
   - Create a file named **`index.html`**
   - Create a file named **`styles.css`**
   - Create a file named **`README.md`**
   - Create a file named **`.gitignore`**

3. **Build your webpage**
   - Write your HTML structure in `index.html`
   - Write your CSS styling in `styles.css`
   - Commit your work to the repository as you progress

4. **Deploy the project to GitHub Server (GitHub Pages)**
5. **Share the link to your public repository** with your instructor in a **direct message** when your project is complete.
---

## Deliverables (check before submitting)
- [ ] Make multiple commits with descriptive messages that explain what and why, not just how.
- [ ] The repository is **public** on GitHub  
- [ ] The repository contains `index.html` and `styles.css`  
- [ ] The webpage includes a **header**, **main**, and **footer**  
- [ ] The webpage includes **at least one table**  
- [ ] The webpage includes **at least one form**  
- [ ] The page is styled using **CSS selectors**  
- [ ] The webpage is **deployed** using GitHub Pages  
- [ ] **Write a report** in **`README.md`** describing what steps you completed to build the project, including how you structured the HTML and how you applied CSS.

---


