<!DOCTYPE html>
<html lang="en">
<head>

<title>EbookHub - Read & Download Free Ebooks</title>
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, sans-serif; }
  body { background: #f4f6fb; color: #222; line-height: 1.6; }

  /* Header */
  header {
    background: linear-gradient(135deg, #6a11cb, #2575fc);
    color: #fff;
    padding: 18px 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  }
  header h1 { font-size: 26px; letter-spacing: 1px; }
  header h1 span { color: #ffd93d; }
  nav a {
    color: #fff;
    margin-left: 25px;
    text-decoration: none;
    font-weight: 500;
    transition: 0.3s;
  }
  nav a:hover { color: #ffd93d; }

  /* Hero */
  .hero {
    background: linear-gradient(135deg, #2575fc, #6a11cb);
    color: #fff;
    text-align: center;
    padding: 70px 20px;
  }
  .hero h2 { font-size: 42px; margin-bottom: 15px; }
  .hero p { font-size: 18px; margin-bottom: 25px; opacity: 0.9; }
  .search-box {
    max-width: 550px;
    margin: 0 auto;
    display: flex;
    background: #fff;
    border-radius: 50px;
    overflow: hidden;
    box-shadow: 0 8px 25px rgba(0,0,0,0.2);
  }
  .search-box input {
    flex: 1;
    padding: 15px 22px;
    border: none;
    outline: none;
    font-size: 16px;
  }
  .search-box button {
    padding: 15px 30px;
    background: #ffd93d;
    color: #222;
    border: none;
    font-weight: bold;
    cursor: pointer;
    transition: 0.3s;
  }
  .search-box button:hover { background: #ffc107; }

  /* Section */
  section { padding: 50px 40px; }
  .section-title {
    text-align: center;
    font-size: 30px;
    margin-bottom: 35px;
    color: #2575fc;
    position: relative;
  }
  .section-title::after {
    content: '';
    width: 70px;
    height: 4px;
    background: #ffd93d;
    display: block;
    margin: 10px auto 0;
    border-radius: 4px;
  }

  /* Books Grid */
  .books-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 25px;
    max-width: 1200px;
    margin: 0 auto;
  }
  .book-card {
    background: #fff;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 6px 18px rgba(0,0,0,0.08);
    transition: 0.3s;
    display: flex;
    flex-direction: column;
  }
  .book-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 12px 28px rgba(0,0,0,0.15);
  }
  .book-cover {
    height: 260px;
    background: linear-gradient(135deg, #6a11cb, #2575fc);
    display: flex;
    align-items: center;
    justify-content: center;
    color: #fff;
    font-size: 60px;
    font-weight: bold;
    position: relative;
  }
  .book-cover::after {
    content: '📖';
    position: absolute;
    bottom: 10px;
    right: 15px;
    font-size: 24px;
    opacity: 0.6;
  }
  .book-info { padding: 18px; flex: 1; display: flex; flex-direction: column; }
  .book-info h3 { font-size: 18px; margin-bottom: 8px; color: #222; }
  .book-info .author { font-size: 14px; color: #777; margin-bottom: 10px; }
  .book-info .rating { color: #ffb400; margin-bottom: 12px; font-size: 14px; }
  .btn-download {
    margin-top: auto;
    display: block;
    text-align: center;
    background: #2575fc;
    color: #fff;
    padding: 10px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    transition: 0.3s;
  }
  .btn-download:hover { background: #6a11cb; }

  /* Footer */
  footer {
    background: #1a1a2e;
    color: #ccc;
    text-align: center;
    padding: 30px 20px;
    margin-top: 40px;
  }
  footer p { margin: 6px 0; font-size: 14px; }
  footer a { color: #ffd93d; text-decoration: none; }

  /* Responsive */
  @media (max-width: 600px) {
    header { flex-direction: column; gap: 10px; padding: 15px; }
    nav a { margin: 0 10px; }
    .hero h2 { font-size: 28px; }
    section { padding: 30px 15px; }
    .section-title { font-size: 24px; }
  }
</style>
</head>
<body>

<header>
  <h1>📚 Ebook<span>Hub</span></h1>
  <nav>
    <a href="#home">Home</a>
    <a href="#books">Ebooks</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<div class="hero" id="home">
  <h2>Read Free Ebooks Anytime, Anywhere</h2>
  <p>Thousands of free ebooks — Download in PDF, EPUB & MOBI format</p>
  <form class="search-box" onsubmit="event.preventDefault(); alert('Search coming soon!');">
    <input type="text" placeholder="Search ebooks by title or author...">
    <button type="submit">Search</button>
  </form>
</div>

<section id="books">
  <h2 class="section-title">Popular Ebooks</h2>
  <div class="books-grid">
    <div class="book-card">
      <div class="book-cover">A</div>
      <div class="book-info">
        <h3>Atomic Habits</h3>
        <p class="author">James Clear</p>
        <p class="rating">★★★★★ (4.9)</p>
        <a class="btn-download" href="#" onclick="alert('Download started!')">⬇ Download</a>
      </div>
    </div>
    <div class="book-card">
      <div class="book-cover">R</div>
      <div class="book-info">
        <h3>Rich Dad Poor Dad</h3>
        <p class="author">Robert Kiyosaki</p>
        <p class="rating">★★★★☆ (4.7)</p>
        <a class="btn-download" href="#" onclick="alert('Download started!')">⬇ Download</a>
      </div>
    </div>
    <div class="book-card">
      <div class="book-cover">P</div>
      <div class="book-info">
        <h3>The Psychology of Money</h3>
        <p class="author">Morgan Housel</p>
        <p class="rating">★★★★★ (4.8)</p>
        <a class="btn-download" href="#" onclick="alert('Download started!')">⬇ Download</a>
      </div>
    </div>
    <div class="book-card">
      <div class="book-cover">I</div>
      <div class="book-info">
        <h3>Ikigai</h3>
        <p class="author">Héctor García</p>
        <p class="rating">★★★★☆ (4.6)</p>
        <a class="btn-download" href="#" onclick="alert('Download started!')">⬇ Download</a>
      </div>
    </div>
    <div class="book-card">
      <div class="book-cover">D</div>
      <div class="book-info">
        <h3>Deep Work</h3>
        <p class="author">Cal Newport</p>
        <p class="rating">★★★★★ (4.7)</p>
        <a class="btn-download" href="#" onclick="alert('Download started!')">⬇ Download</a>
      </div>
    </div>
    <div class="book-card">
      <div class="book-cover">S</div>
      <div class="book-info">
        <h3>The Subtle Art</h3>
        <p class="author">Mark Manson</p>
        <p class="rating">★★★★☆ (4.5)</p>
        <a class="btn-download" href="#" onclick="alert('Download started!')">⬇ Download</a>
      </div>
    </div>
    <div class="book-card">
      <div class="book-cover">7</div>
      <div class="book-info">
        <h3>7 Habits</h3>
        <p class="author">Stephen Covey</p>
        <p class="rating">★★★★★ (4.8)</p>
        <a class="btn-download" href="#" onclick="alert('Download started!')">⬇ Download</a>
      </div>
    </div>
    <div class="book-card">
      <div class="book-cover">M</div>
      <div class="book-info">
        <h3>Mindset</h3>
        <p class="author">Carol Dweck</p>
        <p class="rating">★★★★☆ (4.6)</p>
        <a class="btn-download" href="#" onclick="alert('Download started!')">⬇ Download</a>
      </div>
    </div>
  </div>
</section>

<section id="about">
  <h2 class="section-title">About Us</h2>
  <p style="max-width:800px;margin:0 auto;text-align:center;font-size:17px;color:#555;">
    EbookHub is a free online platform where you can discover, read, and download thousands of ebooks across various categories including Self-Help, Business, Fiction, and more. Our mission is to make knowledge accessible to everyone, everywhere.
  </p>
</section>

<footer id="contact">
  <p>📧 Email: contact@ebookhub.com</p>
  <p>© 2025 EbookHub. All rights reserved.</p>
  <p>Made with ❤️ for readers</p>
</footer>

</body>
</html>
