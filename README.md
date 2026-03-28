
# Instagram Clone

A simple, static clone of Instagram built as a personal learning project.

---

## About

This project is a personal experiment to recreate the look-and-feel of Instagram using only HTML and CSS. The goal was to learn how modern app and website layouts are structured, practice frontend markup and styling, and explore how UI components in a social-media-like interface can be composed.

Important: this is a beginner/learning project — there is no backend, no authentication, and no database. It is intended as a static front-end exercise and portfolio piece.

---

## Features

- Static feed layout with posts (images, captions, likes/comments UI elements)
- Header with logo/search/navigation
- Sidebar/profile card (example layout)
- Comment-like and like-like visual elements (UI-only)
- Responsive-ish layout that demonstrates basic responsive techniques (media queries)
- Clean, semantic HTML structure and separated CSS for styling

---

## Tech Stack

- Frontend: HTML, CSS
- No JavaScript required for the core layout (optional JS can be added later)
- No backend or database — static files only

---

## Getting Started

These instructions will help you run the project locally so you can view and inspect the files.

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, etc.)
- (Optional) A code editor like VS Code

### Quick ways to view the site

1. Clone the repository:
   git clone https://github.com/justayogi/instagram_repo.git

2. Open the project:
   - Option A: Double-click `index.html` to open it directly in your browser.
   - Option B (recommended for consistent behavior): Start a simple local server.

   - Using Python 3:
     python -m http.server 8000
     Then open `http://localhost:8000` in your browser.

   - Using VS Code + Live Server extension:
     - Open the folder in VS Code
     - Right-click `index.html` → "Open with Live Server"

### Project structure (example)
- index.html — main page and layout
- css/
  - styles.css — primary styles
- assets/
  - images/ — images used in the sample posts
- README.md

(Adjust paths above to match your repository if different.)

---

## Example code snippets

Here is a minimal HTML skeleton demonstrating the structure used in this project:

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Instagram Clone</title>
  <link rel="stylesheet" href="css/styles.css" />
</head>
<body>
  <header class="site-header">
    <div class="logo">Instagram Clone</div>
    <nav class="main-nav">
      <!-- nav items -->
    </nav>
  </header>

  <main class="content">
    <aside class="sidebar">
      <!-- profile / suggestions -->
    </aside>

    <section class="feed">
      <article class="post">
        <img src="assets/images/sample-post.jpg" alt="post image" />
        <div class="post-body">
          <h3 class="author">username</h3>
          <p class="caption">This is a sample caption for the post.</p>
        </div>
      </article>
      <!-- more posts -->
    </section>
  </main>
</body>
</html>
```

A simple CSS snippet (in `css/styles.css`) for layout basics:

```css
body {
  font-family: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
  margin: 0;
  background: #fafafa;
  color: #111;
}

.site-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 12px 24px;
  border-bottom: 1px solid #ddd;
  background: #fff;
}

/* Basic grid */
.content {
  display: grid;
  grid-template-columns: 1fr 360px;
  gap: 24px;
  max-width: 1000px;
  margin: 24px auto;
  padding: 0 16px;
}
```

---

## Notes & Limitations

- This is intentionally a static UI project for learning. Interactivity like creating posts, persistent likes, authentication, and real-time updates are not implemented.
- Images used may be placeholders — replace with your own images if desired.
- Consider this a foundation: you can later add JavaScript, a backend, or convert this into a React/Vue app for dynamic behavior.

---

## Contact

If you want to reach out or see more of my work:

- GitHub: https://github.com/justayogi
- LinkedIn: https://www.linkedin.com/in/yogi-patel-489883328/
- Email: yogikanjipatel121@gmail.com

---

## Credits

Built by Yogi Patel as a learning/portfolio project.

---
