<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    outline: none;
    font-family: 'Poppins', sans-serif;
}

html {
    font-size: 62.5%;
}

body {
    width: 100%;
    height: 100vh;
    overflow-x: hidden;
    background-color: #121212;
    color: white;
}

header {
    margin-top: 20px;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 1rem 9%;
    background-color: #121212;
    filter: drop-shadow(10px);
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}


















.logo {
    font-size: 3rem;
    color: #A97155;
    font-weight: 800;
    cursor: pointer;
    transition: 0.5s ease;
}

.logo:hover {
    transform: scale(1.1);
}

.hamburger {
    display: none;
    cursor: pointer;
    font-size: 2.5rem;
    color: white;
}

nav a {
    font-size: 1.8rem;
    color: white;
    margin-left: 4rem;
    font-weight: 500;
    transition: 0.3s ease;
    border-bottom: 3px solid transparent;
}

nav a:hover,
nav a.active {
    color: #A97155;
    color: #A97155;
    border-bottom: 3px solid #A97155;
}














@media(max-width:995px) {
    .hamburger {
        display: block;
    }

    nav {
        position: absolute;
        display: none;
        top: 5rem;
        right: 0;
        width: 40%;
        border-left: 3px solid #A97155;
        border-bottom: 3px solid #A97155;
        border-bottom-left-radius: 2rem;
        padding: 1rem solid;
        background-color: #161616;
        border-top: 0.1rem solid rgba(0, 0, 0, 0.1);
    }

    nav.active {
        display: block;
    }

    nav a {
        display: block;
        font-size: 2rem;
        margin: 3rem 0;
    }

    nav a:hover,
    nav a.active {
        padding: 1rem;
        border-radius: 0.5rem;
        border-bottom: 0.5rem solid #A97155;
    }
}
















section {
    min-height: 100vh;
    padding: 5rem 9% 5rem;
}

.home {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 8rem;
    background-color: black;
}

.home .home-content h1 {
    font-size: 6rem;
    font-weight: 700;
    line-height: 1.3;
}

span {
    color: #D8C4A0;
}

.home-content h3 {
    font-size: 4rem;
    margin-bottom: 1rem;
    font-weight: 700;
}

.home-content p {
    font-size: 1.6rem;
}

.home-img {
    border-radius: 50%;
}






















.home-img img {
    position: relative;
    width: 32vw;
    border-radius: 50%;
    box-shadow: 0 0 25px solid #D8C4A0;
    cursor: pointer;
    transition: 0.2s linear;
}

.home-img img:hover {
    font-size: 1.8rem;
    font-weight: 500;
}

.social-icons a {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 4rem;
    height: 4rem;
    background-color: transparent;
    border: 0.2rem solid #3A5A40;
    font-size: 2rem;
    border-radius: 50%;
    margin: 3rem 1.5rem 3rem 0;
    transition: 0.3s ease;
    color: #3A5A40;
}

.social-icons a:hover {
    color: black;
    transform: scale(1.3) translateY(-5px);
    background-color: #3A5A40;
    box-shadow: 0 0 25px #3A5A40;
}


















.btn {
    display: inline-block;
    padding: 1rem 2.8rem;
    background-color: black;
    border-radius: 4rem;
    font-size: 1.6rem;
    color: #3A5A40;
    letter-spacing: 0.3rem;
    font-weight: 600;
    border: 2px solid #3A5A40;
    transition: 0.3s ease;
    cursor: pointer;
}

.btn:hover {
    transform: scale3d(1.03);
    background-color: #3A5A40;
    color: black;
    box-shadow: 0 0 25px #3A5A40;
}




















@media (max-width: 1000px) {
    .home {
        gap: 4rem;
    }
}

@media(max-width:995px) {
    .home {
        flex-direction: column;
        margin: 5rem 4rem;
    }

    .home .home-content h3 {
        font-size: 2.5rem;
    }

    .home-content h1 {
        font-size: 5rem;
    }

    .home-img img {
        width: 70vw;
        margin-top: 4rem;
    }
}
    <title>Portfolio Website</title>
</head>

<body>

    <header>

        <a href="#" class="logo">Akshat</a>

        <div class="hamburger">
            <i class="fas fa-bars"></i>
        </div>

        <nav>
            <a href="#" class="active">Home</a>
            <a href="#">Services</a>
            <a href="#">Skills</a>
            <a href="#">Education</a>
            <a href="#">Experience</a>
            <a href="#">Contact</a>
        </nav>
        
    </header>
    <section class="home">
        <div class="home-img">
            <img src="main.png" alt="">
        </div>
        <div class="home-content">
            <h1>Hi, It's <span>Akshat Mishra</span></h1>
            <h3 class="typing-text">I'm a <span id="typing"></span></h3>
            <p>
                A storyteller in code, weaving logic with design. React paints the canvas, Node powers the frame, and MongoDB breathes life into data. Every project becomes a journey—interfaces that speak, systems that scale. With curiosity as fuel, the path of a developer is one of endless creation.
            </p>
            <div class="social-icons">
                <a href="www.linkedin.com/in/akshat-mishra-7608ab24a"><i class="fa-brands fa-linkedin"></i></a>
                <a href="https://github.com/akshatmishra1203"><i class="fa-brands fa-github"></i></a>
                <a href="#"><i class="fa-brands fa-x-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
            </div>
            <a href="https://drive.google.com/file/d/14MtrTdMMaQbTAMSshB2W5onta1JDXll2/view?usp=sharing" class="btn">Resume📄</a>
        </div>
    </section>


    <script>
    document.addEventListener('DOMContentLoaded', () => {
    const hamburger = document.querySelector('.hamburger');
    const nav = document.querySelector('nav');

    hamburger.addEventListener('click', () => {
        nav.classList.toggle('active');
    });



























    const typingElement = document.getElementById('typing');
    const words = ["Web Developer", "UI/UX Designer", "Full Stack Developer"];
    let wordIndex = 0;
    let letterIndex = 0;
    let currentWord = '';
    let currentLetters = '';
    let isDeleting = false;
    function type() {
        if (isDeleting) {
            currentLetters = currentWord.substring(0, letterIndex - 1);
            letterIndex--;
        } else {
            currentLetters = currentWord.substring(0, letterIndex + 1);
            letterIndex++;
        }

        typingElement.innerHTML = currentLetters;

        let typeSpeed = 200;
        if (isDeleting) {
            typeSpeed /= 2;
        }

        if (!isDeleting && letterIndex === currentWord.length) {
            typeSpeed = 2000;
            isDeleting = true;
        } else if (isDeleting && letterIndex === 0) {
            isDeleting = false;
            wordIndex++;
            if (wordIndex === words.length) {
                wordIndex = 0;
            }
            currentWord = words[wordIndex];
            typeSpeed = 500;
        }

        setTimeout(type, typeSpeed);
    }
    currentWord = words[wordIndex];
    type();
});

    </script>

</body>

</html>
