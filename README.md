# Final Project and Deployment

## Objectives
Build a fully functional web application.
Apply HTML, CSS, and JavaScript concepts learned.
Deploy the project using GitHub Pages, Netlify, or Vercel.

## Instructions
Choose one of the following project ideas:
Blog Website: Implement a multi-page site with navigation.
Ecommerce Website: Implement a multi-page site with navigation.

>[!NOTE]
> - Include at least:
> - A responsive design.
> - JavaScript interactivity.
> - A deployment link.

## Tasks

Create a well-structured HTML5 document.
Use at least 5 different HTML elements.
Ensure semantic correctness.

Good luck and happy coding! 🚀💻

  E-COMMERCE website 


1. Project Structure
Organize the project with a clear folder structure:

project-folder/
├── index.html
├── about.html
├── blog.html
├── styles.css
├── script.js
├── images/



2. HTML: A Well-Structured and Semantic `index.html`

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Blog</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul class="navigation">
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="blog.html">Blog</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <h1>Welcome to My Blog</h1>
            <p>Sharing thoughts, ideas, and stories with the world.</p>
        </section>

        <section class="latest-posts">
            <h2>Latest Posts</h2>
            <article>
                <h3>How to Build a Blog</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
                <a href="#">Read More</a>
            </article>
            <article>
                <h3>CSS Tips for Beginners</h3>
                <p>Unlock the potential of CSS with these easy tips...</p>
                <a href="#">Read More</a>
            </article>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 My Blog. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>


 

 3. CSS: Responsive Design (`styles.css`)

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    line-height: 1.6;
}

header {
    background: #333;
    color: white;
    padding: 1rem 0;
}

.navigation {
    display: flex;
    justify-content: center;
    list-style: none;
    padding: 0;
}

.navigation li {
    margin: 0 1rem;
}

.navigation a {
    color: white;
    text-decoration: none;
}

.hero {
    text-align: center;
    padding: 2rem;
    background: #f4f4f4;
}

.latest-posts {
    padding: 2rem;
    max-width: 800px;
    margin: 0 auto;
}

@media (max-width: 768px) {
    .navigation {
        flex-direction: column;
        align-items: center;
    }
    .navigation li {
        margin: 0.5rem 0;
    }
}




 4. **JavaScript: Interactivity (`script.js`)

// Example: Dynamic Greeting Based on Time
document.addEventListener("DOMContentLoaded", function() {
    const heroSection = document.querySelector(".hero h1");
    const currentHour = new Date().getHours();
    let greeting;

    if (currentHour < 12) {
        greeting = "Good Morning!";
    } else if (currentHour < 18) {
        greeting = "Good Afternoon!";
    } else {
        greeting = "Good Evening!";
    }

    heroSection.textContent = `${greeting} Welcome to My Blog`;
});

