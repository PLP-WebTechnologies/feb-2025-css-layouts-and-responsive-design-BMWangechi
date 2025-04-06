# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨
Answers
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Test Webpage</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav class="navbar">
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>
    <header class="header">
        <h1>Welcome to My Website</h1>
    </header>
    <main class="main-content">
        <section class="content">
            <h2>Section 1</h2>
            <p>This is some content for section 1.</p>
        </section>
        <section class="content">
            <h2>Section 2</h2>
            <p>This is some content for section 2.</p>
        </section>
        <section class="content">
            <h2>Section 3</h2>
            <p>This is some content for section 3.</p>
        </section>
    </main>
    <footer class="footer">
        <p>&copy; 2025 Your Company</p>
    </footer>
</body>
</html>
/* Basic styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.navbar {
    background-color: #333;
    color: white;
    padding: 1rem;
}

.navbar ul {
    list-style: none;
    display: flex;
    justify-content: space-around;
    margin: 0;
    padding: 0;
}

.navbar a {
    color: white;
    text-decoration: none;
}

.header {
    background-color: #f4f4f4;
    padding: 2rem;
    text-align: center;
}

.main-content {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 2rem;
}

.content {
    background-color: #e4e4e4;
    margin: 1rem;
    padding: 1rem;
    flex: 1 1 30%;
    box-sizing: border-box;
}

.footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 1rem;
}

/* Media Queries */
@media (max-width: 768px) {
    .navbar ul {
        flex-direction: column;
        align-items: center;
    }

    .main-content {
        flex-direction: column;
        align-items: center;
    }

    .content {
        flex: 1 1 80%;
    }
}

@media (max-width: 480px) {
    .content {
        flex: 1 1 100%;
    }
}
