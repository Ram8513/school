# school
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Children Pre school </title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f4;
      color: #333333;
    }
    header {
      background-color: #4CAF50;
      color: white;
      padding: 20px 0;
      text-align: center;
    }
    nav {
      background-color: #333;
      overflow: hidden;
    }
    nav a {
      float: left;
      display: block;
      color: white;
      text-align: center;
      padding: 14px 20px;
      text-decoration: none;
    }
    nav a:hover {
      background-color: #ddd;
      color: black;
    }
    section {
      padding: 20px;
      text-align: center;
    }
    footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 10px 0;
      position: fixed;
      bottom: 0;
      width: 100%;
    }
    .contact-form input, .contact-form textarea {
      width: 80%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .contact-form button {
      padding: 10px 20px;
      background-color: #4CAF50;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .contact-form button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to children pre school</h1>
    <p>where every child shine</p>
  </header>

  <nav>
    <a href="#about">About Us</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="about">
    <h2>About Our School</h2>
    <p>Children pre School is dedicated to providing quality education to students from all backgrounds. Our mission is to nurture creativity, critical thinking, and lifelong learning.</p>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <form class="contact-form" onsubmit="submitForm(event)">
      <input type="text" id="name" placeholder="Your Name" required>
      <input type="ContactNO" id="ContactNo" placeholder="Your contactNo" required>
      <textarea id="message" rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send</button>
    </form>
    <p id="formResponse" style="color: green; margin-top: 10px;"></p>
  </section>

  <footer>
    <p>&copy; 2025 ABC School. All rights reserved.</p>
  </footer>

  <script>
    function submitForm(event) {
      event.preventDefault();
      const name = document.getElementById('name').value;
      const ContactNO = document.getElementById('ContactNO').value;
      const message = document.getElementById('message').value;

      if (name && ContactNO && message) {
        document.getElementById('formResponse').textContent = `Thank you, ${name}! Your message has been received.`;
      } else {
        document.getElementById('formResponse').textContent = 'Please fill out all fields.';
      }
    }
  </script>
</body>
</html>
