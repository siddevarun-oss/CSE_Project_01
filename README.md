# CSE_Project_01
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Varun Academy - Quality Education for All</title>

    <style>
        /* ==========================================
           GLOBAL STYLES
        ========================================== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: white;
            background-color: red;
        }

        /* ==========================================
           HEADER
        ========================================== */
        header {
            background: linear-gradient(135deg, purple 0%, #5a189a 100%);
            color: white;
            padding: 1rem 0;
            position: sticky;
            top: 0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
            z-index: 100;
        }

        .header-container {
            max-width: 1200px;
            margin: auto;
            padding: 0 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .school-name {
            font-size: 1.8rem;
            font-weight: bold;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 2rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: 0.3s;
        }

        nav a:hover {
            color: yellow;
        }

        /* ==========================================
           MAIN
        ========================================== */
        main {
            max-width: 1200px;
            margin: auto;
            padding: 20px;
        }

        section {
            background: rgba(128, 0, 128, 0.9);
            margin: 2rem 0;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.3);
        }

        h1, h2 {
            text-align: center;
            margin-bottom: 1rem;
        }

        h2 {
            border-bottom: 3px solid white;
            padding-bottom: 10px;
        }

        /* ==========================================
           BANNER
        ========================================== */
        .banner {
            width: 100%;
            height: 300px;
            background: linear-gradient(135deg, purple 0%, #9d4edd 100%);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            font-weight: bold;
            margin-bottom: 2rem;
            text-align: center;
        }

        .welcome-message {
            text-align: center;
            font-size: 1.2rem;
            margin-bottom: 1rem;
        }

        .welcome-btn {
            display: block;
            margin: auto;
            background: white;
            color: purple;
            padding: 12px 25px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: 0.3s;
        }

        .welcome-btn:hover {
            background: yellow;
            transform: scale(1.05);
        }

        /* ==========================================
           FEATURES
        ========================================== */
        .about-features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .feature-box {
            background: rgba(255,255,255,0.2);
            padding: 1.5rem;
            border-radius: 8px;
            transition: 0.3s;
        }

        .feature-box:hover {
            transform: translateY(-5px);
            background: rgba(255,255,255,0.3);
        }

        /* ==========================================
           COURSES
        ========================================== */
        .courses-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px,1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .course-card {
            background: white;
            color: #333;
            border-radius: 10px;
            padding: 1.5rem;
            transition: 0.3s;
        }

        .course-card:hover {
            transform: translateY(-10px);
        }

        .course-card h3 {
            color: purple;
        }

        .course-badge {
            display: inline-block;
            margin-top: 10px;
            background: purple;
            color: white;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
        }

        /* ==========================================
           CONTACT FORM
        ========================================== */
        .contact-form {
            max-width: 500px;
            margin: auto;
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        .form-group {
            display: flex;
            flex-direction: column;
        }

        label {
            margin-bottom: 5px;
            font-weight: bold;
        }

        input,
        textarea {
            padding: 12px;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
        }

        textarea {
            min-height: 120px;
        }

        .submit-btn {
            background: white;
            color: purple;
            padding: 12px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: 0.3s;
        }

        .submit-btn:hover {
            background: yellow;
        }

        /* ==========================================
           FOOTER
        ========================================== */
        footer {
            background: purple;
            text-align: center;
            padding: 2rem;
            margin-top: 2rem;
        }

        /* ==========================================
           RESPONSIVE DESIGN
        ========================================== */
        @media (max-width: 768px) {

            .header-container {
                flex-direction: column;
                gap: 1rem;
            }

            nav ul {
                flex-direction: column;
                text-align: center;
                gap: 1rem;
            }

            .banner {
                height: 200px;
                font-size: 1.5rem;
            }
        }
    </style>
</head>

<body>

    <!-- HEADER -->
    <header>
        <div class="header-container">
            <h1 class="school-name">📚 Varun Academy</h1>

            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#courses">Courses</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- MAIN -->
    <main>

        <!-- HOME -->
        <section id="home">
            <div class="banner">
                🎓 Welcome to Varun Academy
            </div>

            <h1>Quality Education for All</h1>

            <p class="welcome-message">
                Welcome to Varun Academy, where we believe in providing
                quality education to every student with modern teaching methods.
            </p>

            <button class="welcome-btn" onclick="showWelcomeMessage()">
                ✨ Click to Explore!
            </button>
        </section>

        <!-- ABOUT -->
        <section id="about">
            <h2>About Our Academy</h2>

            <p>
                Varun Academy has been serving students with excellent
                education and modern learning facilities. Our mission
                is to help every student succeed.
            </p>

            <div class="about-features">

                <div class="feature-box">
                    <h3>🎯 Expert Teachers</h3>
                    <p>Highly experienced teachers for quality learning.</p>
                </div>

                <div class="feature-box">
                    <h3>🏫 Modern Facilities</h3>
                    <p>Advanced classrooms, labs, and digital learning.</p>
                </div>

                <div class="feature-box">
                    <h3>🌟 Student Growth</h3>
                    <p>Focus on academics, sports, and creativity.</p>
                </div>

            </div>
        </section>

        <!-- COURSES -->
        <section id="courses">
            <h2>Our Courses</h2>

            <div class="courses-grid">

                <div class="course-card">
                    <h3>📐 Mathematics</h3>
                    <p>Learn algebra, geometry, and advanced mathematics.</p>
                    <span class="course-badge">Grades 1-12</span>
                </div>

                <div class="course-card">
                    <h3>🔬 Science</h3>
                    <p>Practical learning in physics, chemistry, and biology.</p>
                    <span class="course-badge">Grades 1-12</span>
                </div>

                <div class="course-card">
                    <h3>🌍 English</h3>
                    <p>Improve grammar, writing, and communication skills.</p>
                    <span class="course-badge">Grades 1-12</span>
                </div>

                <div class="course-card">
                    <h3>💻 Computer Science</h3>
                    <p>Programming and web development for modern careers.</p>
                    <span class="course-badge">Grades 6-12</span>
                </div>

            </div>
        </section>

        <!-- CONTACT -->
        <section id="contact">
            <h2>Contact Us</h2>

            <form class="contact-form" onsubmit="submitForm(event)">

                <div class="form-group">
                    <label>Your Name</label>
                    <input type="text" required>
                </div>

                <div class="form-group">
                    <label>Your Email</label>
                    <input type="email" required>
                </div>

                <div class="form-group">
                    <label>Your Message</label>
                    <textarea required></textarea>
                </div>

                <button type="submit" class="submit-btn">
                    Send Message
                </button>

            </form>
        </section>

    </main>

    <!-- FOOTER -->
    <footer>
        <p>
            © 2026 Varun Academy | All Rights Reserved
        </p>
    </footer>

    <!-- JAVASCRIPT -->
    <script>

        function showWelcomeMessage() {
            alert(
                "🎉 Welcome to Varun Academy!\n\nWe are happy to have you here."
            );
        }

        function submitForm(event) {
            event.preventDefault();

            alert("✅ Message Sent Successfully!");

            document.querySelector(".contact-form").reset();
        }

    </script>

</body>
</html>
