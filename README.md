<!DOCTYPE html>
<html lang="{{ shop.locale }}">
<head>
  <meta charset="utf-8">
  <title>{{ page_title }}</title>
  <meta name="description" content="{{ page_description }}">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <link href="{{ 'styles.css' | asset_url }}" rel="stylesheet">
  {{ content_for_header }}
</head>
<body>
  <header>
    <div class="header-container">
      <div class="logo">
        <a href="{{ shop.url }}">{{ shop.name }}</a>
      </div>
      <div class="search-bar">
        <input type="text" placeholder="Search products...">
        <button type="submit">Search</button>
      </div>
      <div class="user-actions">
        <a href="/account">My Account</a>
        <a href="/cart">Cart</a>
      </div>
    </div>
  </header>
  <nav>
    <ul class="main-menu">
      <li><a href="/">Home</a></li>
      <li><a href="/collections">Shop</a></li>
      <li><a href="/about">About Us</a></li>
      <li><a href="/contact">Contact</a></li>
    </ul>
  </nav>
  <main>
    {{ content_for_layout }}
  </main>
  <footer>
    <div class="footer-container">
      <ul class="footer-menu">
        <li><a href="/">Home</a></li>
        <li><a href="/collections">Shop</a></li>
        <li><a href="/about">About Us</a></li>
        <li><a href="/contact">Contact</a></li>
      </ul>
      <div class="social-links">
        <!-- Add your social media links here -->
      </div>
    </div>
  </footer>
</body>
</html>
