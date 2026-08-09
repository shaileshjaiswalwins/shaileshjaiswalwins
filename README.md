cd ~
git clone https://github.com/shaileshjaiswalwins/shaileshjaiswalwins.github.io.git
cd shaileshjaiswalwins.github.io
cat > index.html << 'EOF'
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Shailesh Jaiswal</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Shailesh Jaiswal</h1>
    <p class="tagline">Bangalore &middot; Building with AI</p>
    <nav>
      <a href="https://github.com/shaileshjaiswalwins">GitHub</a>
      <a href="https://linkedin.com/in/shaileshjaiswalwins">LinkedIn</a>
    </nav>
  </header>
  <main>
    <section id="about">
      <h2>About</h2>
      <p>This is my personal site, where I share what I'm building and learning. Updated regularly as new projects and notes get added.</p>
    </section>
    <section id="projects">
      <h2>Projects</h2>
      <ul class="project-list">
        <li><strong>Coming soon</strong><p>Add your first project here.</p></li>
      </ul>
    </section>
    <section id="log">
      <h2>Log</h2>
      <ul class="log-list">
        <li><time datetime="2026-08-09">2026-08-09</time> — Site scaffolded. First commit.</li>
      </ul>
    </section>
  </main>
  <footer>
    <p>&copy; 2026 Shailesh Jaiswal</p>
  </footer>
</body>
</html>
EOF
cat > style.css << 'EOF'
:root { --bg: #0d1117; --fg: #e6edf3; --muted: #8b949e; --accent: #58a6ff; }
* { box-sizing: border-box; }
body { margin: 0; font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif; background: var(--bg); color: var(--fg); line-height: 1.6; }
header { padding: 3rem 1.5rem 1.5rem; text-align: center; border-bottom: 1px solid #21262d; }
header h1 { margin: 0 0 0.25rem; font-size: 2rem; }
.tagline { color: var(--muted); margin: 0 0 1rem; }
nav a { color: var(--accent); text-decoration: none; margin: 0 0.75rem; }
nav a:hover { text-decoration: underline; }
main { max-width: 640px; margin: 0 auto; padding: 2rem 1.5rem; }
section { margin-bottom: 2.5rem; }
h2 { font-size: 1.1rem; text-transform: uppercase; letter-spacing: 0.05em; color: var(--muted); border-bottom: 1px solid #21262d; padding-bottom: 0.5rem; }
.project-list, .log-list { list-style: none; padding: 0; }
.project-list li, .log-list li { padding: 0.75rem 0; border-bottom: 1px solid #161b22; }
.log-list time { color: var(--muted); font-size: 0.85rem; }
footer { text-align: center; padding: 2rem 1.5rem; color: var(--muted); font-size: 0.85rem; }
EOF
git add index.html style.css
git commit -m "Add starter site"
git push
