# CODING-SAMURAI-INTERNSHIP-TASK1
‎Project1.html‎
+195
Lines changed: 195 additions & 0 deletions
Original file line number	Diff line number	Diff line change
@@ -0,0 +1,195 @@
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>FoodieHub Portfolio</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #fff8f0;
      color: #333;
      scroll-behavior: smooth;
    }
    header {
      background: linear-gradient(45deg, #ff7043, #ffab91);
      color: white;
      padding: 20px 0;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    nav a {
      margin: 0 15px;
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #ffe0b2;
    }
    section {
      padding: 50px 20px;
      text-align: center;
    }
    #about img {
      width: 200px;
      border-radius: 50%;
      border: 5px solid #ff7043;
      margin-bottom: 15px;
    }
    .recipes, .projects {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
    }
    .card {
      background: white;
      border-radius: 12px;
      box-shadow: 0 6px 12px rgba(0,0,0,0.1);
      width: 280px;
      padding: 20px;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .card:hover {
      transform: translateY(-8px);
      box-shadow: 0 12px 20px rgba(0,0,0,0.2);
    }
    .card img {
      width: 100%;
      border-radius: 12px;
      margin-bottom: 10px;
    }
    form {
      max-width: 400px;
      margin: auto;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }
    input, textarea {
      padding: 12px;
      border: 1px solid #ddd;
      border-radius: 8px;
      font-size: 1em;
    }
    button {
      padding: 12px;
      background: #ff7043;
      color: white;
      border: none;
      cursor: pointer;
      border-radius: 8px;
      font-weight: bold;
      transition: background 0.3s;
    }
    button:hover {
      background: #e64a19;
    }
    footer {
      background: #333;
      color: white;
      text-align: center;
      padding: 20px;
    }
  </style>
</head>
<body>
  <header>
    <h1>🍴 FoodieHub Portfolio</h1>
    <p>"Blending Technology & Taste – Where Code Meets Cuisine"</p>
    <nav>
      <a href="#about">About</a>
      <a href="#recipes">Recipes</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>
  <section id="about">
    <h2>About Me 👩‍🍳</h2>
    <img src="C:\Users\Gundeboina swethaz\Documents\chinnu\food.jpg" alt="Profile">
    <p>Hi!   
       I believe food brings joy, and technology spreads that joy across the globe.  
       From cooking cheesy pizzas 🍕 to coding interactive websites 🌐 – I do it all with love. ❤️</p>
  </section>
  <section id="recipes">
    <h2>My Recipes 🍲</h2>
    <p>Cooking is not just about ingredients – it’s about stories, culture, and memories.  
       Here are some of my favorite creations:</p>
    <div class="recipes">
      <div class="card">
        <img src="C:\Users\Gundeboina swethaz\Documents\chinnu\pizza.jpg" alt="Pizza">
        <h3>Cheesy Pizza</h3>
        <p>A golden crust topped with gooey cheese, fresh tomatoes, and basil –  
           a perfect Italian classic baked with love.</p>
      </div>
      <div class="card">
        <img src="C:\Users\Gundeboina swethaz\Documents\chinnu\pasta.jpg" alt="Pasta">
        <h3>Italian Pasta</h3>
        <p>Rich creamy Alfredo pasta served with garlic bread –  
           comfort food for the soul.</p>
      </div>
      <div class="card">
        <img src="C:\Users\Gundeboina swethaz\Documents\chinnu\Dessert.jpeg" alt="Dessert">
        <h3>Chocolate Lava Cake</h3>
        <p>A warm cake with molten chocolate inside –  
           one bite and you’ll be in dessert heaven. 🍫</p>
      </div>
    </div>
  </section>
  <section id="projects">
    <h2>Projects 👩‍💻</h2>
    <p>As a developer, I love merging my passion for food with technology.  
       Here’s a glimpse of my work:</p>
    <div class="projects">
      <div class="card">
        <img src="https://source.unsplash.com/400x200/?website,design" alt="Blog Website">
        <h3>Food Blog Website</h3>
        <p>A website where I share recipes, kitchen hacks, and food photography.  
           Built using HTML, CSS & JavaScript.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x200/?mobile,app" alt="App">
        <h3>Recipe Finder App</h3>
        <p>A mobile app that suggests recipes based on ingredients you have at home.  
           Cook smart, waste less!</p>
      </div>
    </div>
  </section>
  <section id="contact">
    <h2>Contact Me 📬</h2>
    <p>Got a recipe suggestion, a project idea, or just want to say hi?  
       I’d love to hear from you!</p>
    <form id="contactForm">
      <input type="text" id="name" placeholder="Your Name" required>
      <input type="email" id="email" placeholder="Your Email" required>
      <textarea id="message" rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
    <p id="formMessage"></p>
  </section>
  <footer>
    <p>© 2025 FoodieHub | Made with ❤️ by Swetha</p>
  </footer>
  <script>
    document.getElementById("contactForm").addEventListener("submit", function(e) {
      e.preventDefault();
      let name = document.getElementById("name").value;
      document.getElementById("formMessage").innerText = 
        "Thanks, " + name + "! Your message has been sent. I’ll reply soon. 😊";
      this.reset();
    });
  </script>
</body>
</html>
