
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Luxury Portfolio</title>
    <style>
        /* Reset and base styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Playfair Display', serif; /* Elegant serif font; load from Google Fonts if needed */
            background-color: #000; /* Black background for luxury */
            color: #f5f5f5; /* Off-white text */
            line-height: 1.6;
            overflow-x: hidden;
        }
        a {
            color: #d4af37; /* Gold links */
            text-decoration: none;
        }
        a:hover {
            color: #ffd700; /* Brighter gold on hover */
        }

        /* Header */
        header {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(0, 0, 0, 0.9);
            padding: 1rem 2rem;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.5);
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        nav h1 {
            font-size: 1.5rem;
            color: #d4af37;
        }
        nav ul {
            list-style: none;
            display: flex;
        }
        nav li {
            margin-left: 2rem;
        }
        nav a {
            font-weight: bold;
            transition: color 0.3s;
        }

        /* Sections */
        section {
            min-height: 100vh;
            padding: 5rem 2rem;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
        }
        .hero {
            background: linear-gradient(135deg, #000, #1a1a1a);
        }
        .about, .portfolio, .contact {
            background: #000;
        }
        h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: #d4af37;
        }
        p {
            max-width: 600px;
            margin-bottom: 2rem;
        }

        /* Hero specific */
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        .hero p {
            font-size: 1.2rem;
        }

        /* Portfolio grid */
        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            width: 100%;
        }
        .project {
            background: #1a1a1a;
            padding: 1rem;
            border-radius: 8px;
            box-shadow: 0 4px 20px rgba(212, 175, 55, 0.2);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .project:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 30px rgba(212, 175, 55, 0.4);
        }
        .project img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 4px;
        }

        /* Contact form */
        form {
            max-width: 500px;
            width: 100%;
        }
        input, textarea {
            width: 100%;
            padding: 1rem;
            margin-bottom: 1rem;
            background: #1a1a1a;
            border: 1px solid #d4af37;
            border-radius: 4px;
            color: #f5f5f5;
        }
        button {
            background: #d4af37;
            color: #000;
            padding: 1rem 2rem;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-weight: bold;
            transition: background 0.3s;
        }
        button:hover {
            background: #ffd700;
        }

        /* Footer */
        footer {
            background: #000;
            padding: 2rem;
            text-align: center;
        }

        /* Responsive */
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
                align-items: center;
            }
            nav li {
                margin: 0.5rem 0;
            }
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <h1>My Portfolio</h1>
            <ul>
                <li><a href="#hero">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#portfolio">Work</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="hero" class="hero">
        <h1>Welcome to My World</h1>
        <p>Discover elegance in every detail. I'm a [Your Profession, e.g., Designer/Photographer/Developer] crafting luxurious experiences.</p>
        <a href="#about">Explore</a>
    </section>

    <section id="about" class="about">
        <h2>About Me</h2>
        <p>With a passion for [your niche, e.g., minimalist design and timeless aesthetics], I create portfolios that exude sophistication. My work blends simplicity with luxury, ensuring every project tells a story of refinement.</p>
        <!-- Add a placeholder image or your photo -->
        <img src="https://via.placeholder.com/300x300?text=Your+Photo" alt="Your Photo" style="border-radius: 50%; margin-top: 2rem;">
    </section>

    <section id="portfolio" class="portfolio">
        <h2>My Work</h2>
        <div class="portfolio-grid">
            <div class="project">
                <img src="https://via.placeholder.com/400x300?text=Project+1" alt="Project 1">
                <h3>Project Title 1</h3>
                <p>A luxurious [brief description].</p>
            </div>
            <div class="project">
                <img src="https://via.placeholder.com/400x300?text=Project+2" alt="Project 2">
                <h3>Project Title 2</h3>
                <p>Elegant and timeless.</p>
            </div>
            <!-- Add more projects as needed -->
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>Get in Touch</h2>
        <p>Let's discuss your next luxury project.</p>
        <form action="#" method="post">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2023 My Portfolio. All rights reserved.</p>
    </footer>

    <script>
        // Simple smooth scroll for nav links
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                target.scrollIntoView({ behavior: 'smooth' });
            });
        });
    </script>
</body>
</html>
