 Assignment-3.4.md — Semantic HTML & Accessibility,1. Updated semantic HTML (index.html)

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="A sample webpage demonstrating semantic HTML and accessibility.">
    <title>Semantic HTML & Accessibility</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            color: #222;
            background: #f4f4f4;
        }

        header, nav, main, section, article, aside, footer {
            padding: 16px;
            margin: 10px;
        }

        header, footer {
            background: #243447;
            color: white;
        }

        nav {
            background: #e1e8ef;
        }

        nav a {
            margin-right: 15px;
            color: #123d68;
        }

        main {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 12px;
        }

        section, article, aside {
            background: white;
            border: 1px solid #ccc;
            border-radius: 6px;
        }

        img {
            max-width: 100%;
            height: auto;
        }

        a:focus {
            outline: 3px solid #d97706;
            outline-offset: 3px;
        }

        @media (max-width: 600px) {
            main {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>Welcome to My Website</h1>
        <p>Learning Semantic HTML and Web Accessibility</p>
    </header>

    <nav aria-label="Main navigation">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#articles">Articles</a>
        <a href="#contact">Contact</a>
    </nav>

    <main id="home">
        <section id="about" aria-labelledby="about-heading">
            <h2 id="about-heading">About This Website</h2>
            <p>
                This webpage demonstrates how semantic HTML elements
                improve page structure, accessibility, and readability.
            </p>

            <img
                src="https://placehold.co/600x250?text=Semantic+HTML"
                alt="Illustration representing semantic HTML structure"
                width="600"
                height="250"
            >
        </section>

        <aside aria-labelledby="aside-heading">
            <h2 id="aside-heading">Quick Information</h2>
            <p>
                Semantic elements describe the purpose of webpage
                content and help assistive technologies understand it.
            </p>
        </aside>

        <section id="articles" aria-labelledby="articles-heading">
            <h2 id="articles-heading">Latest Articles</h2>

            <article>
                <h3>Introduction to Semantic HTML</h3>
                <p>
                    Semantic HTML uses meaningful elements such as
                    header, nav, main, article, and footer.
                </p>
                <a href="#contact">Learn more about this website</a>
            </article>

            <article>
                <h3>Why Accessibility Matters</h3>
                <p>
                    Accessible webpages help people with different
                    abilities navigate and understand online content.
                </p>
            </article>
        </section>
    </main>

    <footer id="contact">
        <h2>Contact</h2>
        <p>Contact us for more information about HTML and accessibility.</p>
        <p>&copy; 2026 My Website. All rights reserved.</p>
    </footer>

</body>
</html>
2. Assignment checklist

Used semantic elements: <header>, <nav>, <main>, <section>, <article>, <aside>, and <footer>.

Placed navigation links inside <nav>.

Organized primary content inside <main>.

Maintained a logical heading hierarchy from <h1> to <h3>.

Added descriptive alternative text to the image.

Used meaningful link text and section IDs.

Added keyboard focus styling and responsive layout.
3. Before-and-after screenshots
Before: Open your original div-based webpage in a browser and capture a screenshot.

After: Save the updated code as index.html, open it in a browser, and capture the resulting webpage.

Save both screenshots in your assignment folder, for example:


text
Assignment-3.4/
├── index.html
├── Assignment-3.4.md
└── screenshots/
    ├── before.png
    └── after.png
