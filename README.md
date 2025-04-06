<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Responsive Webpage</title>
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
    <h1>Welcome to Our Website</h1>
  </header>
  <main class="content">
    <section>
      <h2>Section 1</h2>
      <p>Content for section 1.</p>
    </section>
    <section>
      <h2>Section 2</h2>
      <p>Content for section 2.</p>
    </section>
  </main>
  <footer class="footer">
    <p>&copy; 2025 Your Company</p>
  </footer>
</body>
</html>


CSS
/* styles.css */

/* Reset some default styles */
body, h1, h2, p, ul {
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
}

/* Grid layout for the page */
body {
  display: grid;
  grid-template-areas:
    "nav"
    "header"
    "content"
    "footer";
  grid-template-rows: auto;
}

.navbar {
  grid-area: nav;
  background: #333;
}

.navbar ul {
  display: flex;
  justify-content: center;
  list-style: none;
}

.navbar a {
  display: block;
  color: white;
  padding: 15px 20px;
  text-decoration: none;
}

.header {
  grid-area: header;
  background: #f4f4f4;
  padding: 20px;
  text-align: center;
}

.content {
  grid-area: content;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  padding: 20px;
}

.footer {
  grid-area: footer;
  background: #333;
  color: white;
  text-align: center;
  padding: 10px 0;
}

section {
  background: #f4f4f4;
  padding: 20px;
}
