# HTML-CSS-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="styles.css" rel="stylesheet">
    <title>Personal Portfolio Website</title>
</head>
<body>
    <header>
        <div class="header__container">
            <h1 class="header__title">Hey I am [Your Name]</h1>
            <nav class="nav__bar">
                <ul>
                    <li><a class="nav__links" href="#welcome-section">About</a></li>
                    <li><a class="nav__links" href="#projects">Work</a></li>
                    <li><a class="nav__links" href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>
        <section class="section__projects" id="projects">
            <h2>These are some of my projects</h2>
            <div class="projects__div">
                <a href="https://codepen.io/freeCodeCamp/full/zNqgVx" target="_blank" class="project-tile">
                    <img class="projects__images" src="https://cdn.freecodecamp.org/testable-projects-fcc/images/tribute.jpg">
                    <p class="projects__p">Tribute Page</p>
                </a>
                <a href="https://codepen.io/freeCodeCamp/full/qRZeGZ" target="_blank" class="project-tile">
                    <img class="projects__images" src="https://cdn.freecodecamp.org/testable-projects-fcc/images/random-quote-machine.png">
                    <p class="projects__p">Random Quote Machine</p>
                </a>
                <!-- Add more project links here -->
            </div>
        </section>
    </main>

    <!-- Add contact section here -->
</body>
</html>

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-size: 1.5rem;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}

:root {
    /* COLORS */
    --HEADER-RED: rgb(241, 92, 92);
    --FONT-COLOR: whitesmoke;
    --BODY-GRAY: rgb(70, 70, 71);
    --HEADER-HOVER-BLUE: rgb(98, 98, 236);
    --PROJECT-PBGCOLOR: rgb(52, 53, 58);
    --POPPING-RED: brown;
}

/* UTILITY CLASSES */
.wrap {
    white-space: wrap;
}

.inline {
    display: inline;
}

/* || HEADER */
.header__container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
    background-color: var(--HEADER-RED);
}

.header__title {
    font-size: 2rem;
    color: var(--FONT-COLOR);
}

.nav__bar {
    display: flex;
    justify-content: space-between;
}

.nav__bar ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
}

.nav__bar li {
    margin-right: 20px;
}

.nav__links {
    color: var(--FONT-COLOR);
    text-decoration: none;
}

.nav__links:hover {
    color: var(--HEADER-HOVER-BLUE);
}
