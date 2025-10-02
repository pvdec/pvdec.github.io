<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio – 3D Modeling Projects</title>
    <style>
        body {
            font-family: Monospace, Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: #ffffff;
            color: #ffffff;
        }
        header, footer {
            font-family: Monospace, Arial, sans-serif;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: #2a2a2a;
            color: #f5f5f5;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }
        header h1 {
            margin: 0;
            font-size: 2.5rem;
        }
        header p {
            font-size: 1.2rem;
            margin-top: .5rem;
        }
        nav {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: rgb(255, 255, 255);
            padding: 1rem 0;
            box-shadow: 0 2px 5px rgba(255, 255, 255, 0.2);
            display: flex;
            justify-content: center;
        }

        nav button {
            font-family: Monospace, Arial, sans-serif;
            background-color: white;
            color: rgb(14, 14, 14);
            border: none;
            padding: 0.5rem 1rem;
            margin: 0 0.5rem;
            border-radius: 4px;
            cursor: pointer;
            font-size: 1rem;
            outline: 2px solid black;
        }

        nav button:hover {
            background-color: rgb(202, 202, 202);
        }
        .container {
            max-width: 1400px;
            margin: 2rem auto;
            padding: 0 1rem;
        }
        .projectGD {
            background: #8f2121;
            border-radius: 8px;
            padding: 1.5rem;
            margin-bottom: 2rem;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
        }
        .project3D {
            background: #dc9133;
            border-radius: 8px;
            padding: 1.5rem;
            margin-bottom: 2rem;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
        }
        .projectDM {
            background: #66226c;
            border-radius: 8px;
            padding: 1.5rem;
            margin-bottom: 2rem;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
        }
        .projectUI {
            background: #0b6a42;
            border-radius: 8px;
            padding: 1.5rem;
            margin-bottom: 2rem;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
        }
        .projectF {
            background: #0c4867;
            border-radius: 8px;
            padding: 1.5rem;
            margin-bottom: 2rem;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
        }
        .project {
            background: #00000056;
            border-radius: 8px;
            padding: 1.5rem;
            margin-bottom: 2rem;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
        }
        .project h2 {
            margin-top: 0;
            color: #ffffff;
        }
        .project p {
            margin: .5rem 0 1rem;
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
        }
        .gallery img {
            width: 100%;
            border-radius: 6px;
            object-fit: cover;
            box-shadow: none; /* Removed glowing effect */
            cursor: pointer;
        }
        footer {
            text-align: center;
            padding: 1rem;
            background: #ffffff;
            color: black;
            margin-top: 1rem;
        }

        .scroll-gallery {
            display: flex;
            overflow-x: auto;
            gap: 1rem;
            padding-bottom: 1rem;
        }
        .scroll-gallery img {
            max-width: 1000px;
            height: auto;
            object-fit: contain; /* Ensures the entire image fits within the specified size without cropping */
            border-radius: 6px;
            cursor: pointer;
            max-height: 500px;
        }

        .center-gallery {
            display: flex;
            justify-content: center;
            gap: 1rem;
        }

        .center-gallery img {
            max-width: 400px;
            height: auto;
            justify-content: contain; /* Ensures the entire image fits within the specified size without cropping */
            border-radius: 6px;
            box-shadow: none; /* Removed glowing effect */
            cursor: pointer;
            max-height: 400px;
        }

        .fullscreen {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.9);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .fullscreen img {
            max-width: 90%;
            max-height: 90%;
        }

        .fullscreen:target {
            display: flex;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <button onclick="document.getElementById('projectGD').scrollIntoView({ behavior: 'smooth' });">Graphic Design</button>
            <button onclick="document.getElementById('project3D').scrollIntoView({ behavior: 'smooth' });">3D Modeling</button>
            <button onclick="document.getElementById('projectDM').scrollIntoView({ behavior: 'smooth' });">Digital Marketing</button>
            <button onclick="document.getElementById('projectUI').scrollIntoView({ behavior: 'smooth' });">UI Design</button>
            <button onclick="document.getElementById('projectF').scrollIntoView({ behavior: 'smooth' });">Freelance</button>
        </nav>
    </header>

    <div class="container">
        <div class="projectGD" id="projectGD">
            <h2>Graphic Design</h2>
            <p>A university project where I had to create the branding for a fake festival happening in Norway.</p>
            <div class="project">
                <h3>Logos</h3>
                <div class="scroll-gallery">
                    <img src="uniwork/Graphic_Design/Icon/1.png" alt="Logo 1">
                    <img src="uniwork/Graphic_Design/Icon/2.png" alt="Logo 2">
                    <img src="uniwork/Graphic_Design/Icon/3.png" alt="Logo 3">
                    <img src="uniwork/Graphic_Design/Icon/4.png" alt="Logo 4">
                    <img src="uniwork/Graphic_Design/Icon/5.png" alt="Logo 5">
                    <img src="uniwork/Graphic_Design/Icon/6.png" alt="Logo 6">
                </div>
            </div>

            <div class="project">
                <h3>Banner advertisements</h3>
                <div class="scroll-gallery">
                    <img src="uniwork/Graphic_Design/Ads/1.png" alt="Poster 1">
                    <img src="uniwork/Graphic_Design/Ads/4.png" alt="Poster 3">
                    <img src="uniwork/Graphic_Design/Ads/3.png" alt="Poster 1">
                </div>
            </div>

            <div class="project">
                <h3>Brochure</h3>
                <div class="scroll-gallery">
                    <img src="uniwork/Graphic_Design/Brochure/B2.png" alt="Poster 1">
                    <img src="uniwork/Graphic_Design/Brochure/B1.png" alt="Poster 1">
                </div>
            </div>

            <div class="project">
                <h3>Color choice and typography</h3>
                <div class="scroll-gallery">
                    <img src="uniwork/Graphic_Design/Profile/profile-1.png" alt="Poster 1">
                    <img src="uniwork/Graphic_Design/Profile/profile-2.png" alt="Poster 1">
                    <img src="uniwork/Graphic_Design/Profile/profile-3.png" alt="Poster 1">
                    <img src="uniwork/Graphic_Design/Profile/profile-4.png" alt="Poster 1">
                    <img src="uniwork/Graphic_Design/Profile/profile-5.png" alt="Poster 1">
                </div>
            </div>
            <div class="project">
                <h3>Tickets</h3>
                <div class="scroll-gallery">
                    <img src="uniwork/Graphic_Design/Ticket/1.png" alt="Poster 1">
                    <img src="uniwork/Graphic_Design/Ticket/2.png" alt="Poster 1">
                    <img src="uniwork/Graphic_Design/Ticket/3.png" alt="Poster 1">
                </div>
            </div>
        </div>
        <div class="project3D" id="project3D">
            <h2>3D Modeling</h2>
            <p>A collection of diverse university projects.</p>
        <div class="project">
            <h2>Ukelele</h2>
            <div class="scroll-gallery">
                <img src="uniwork/3D Modelling/oblig1DiogoParcerias/1.jpg" alt="Ukulele render">
                <img src="uniwork/3D Modelling/oblig1DiogoParcerias/4.jpg" alt="Ukulele render">
                <img src="uniwork/3D Modelling/oblig1DiogoParcerias/3.jpg" alt="Ukulele render">
                <img src="uniwork/3D Modelling/oblig1DiogoParcerias/2.jpg" alt="Ukulele render">
            </div>
        </div>
        <div class="project">
            <h2>Exploration of interior design - Bedroom</h2>
            <div class="scroll-gallery">
                <img src="uniwork/3D Modelling/oblig2DiogoParcerias/1.jpg" alt="Oblig2 render">
                <img src="uniwork/3D Modelling/oblig2DiogoParcerias/2.jpg" alt="Oblig2 render">
                <img src="uniwork/3D Modelling/oblig2DiogoParcerias/3.jpg" alt="Oblig2 render">
            </div>
        </div>

        <div class="project">
            <h2>Pac-Man</h2>
            <div class="scroll-gallery">
                <img src="uniwork/3D Modelling/Oblig3DiogoParcerias/1.jpg" alt="Oblig3 render">
                <img src="uniwork/3D Modelling/Oblig3DiogoParcerias/2.jpg" alt="Oblig3 render">
                <img src="uniwork/3D Modelling/Oblig3DiogoParcerias/3.jpg" alt="Oblig3 render">
                <img src="uniwork/3D Modelling/Oblig3DiogoParcerias/4.jpg" alt="Oblig3 render">
                <img src="uniwork/3D Modelling/Oblig3DiogoParcerias/5.jpg" alt="Oblig3 render">
                <img src="uniwork/3D Modelling/Oblig3DiogoParcerias/6.jpg" alt="Oblig3 render">
                <img src="uniwork/3D Modelling/Oblig3DiogoParcerias/7.jpg" alt="Oblig3 render">
                <img src="uniwork/3D Modelling/Oblig3DiogoParcerias/8.jpg" alt="Oblig3 render">
            </div>
        </div>
    </div>
    <div class="projectDM" id="projectDM">
        <h2>Digital Marketing</h2>
        <p>A university project where I had to create a marketing campaign for the nordic energry drink "Explo".</p>
        <div class="project">
            <h3>Digital Marketing</h3>
            <div class="scroll-gallery">
                <img src="uniwork/Digital%20Marketing/6.jpg" alt="Poster 1">
                <img src="uniwork/Digital%20Marketing/2.png" alt="Poster 1">
                <img src="uniwork/Digital%20Marketing/4.png" alt="Poster 1">
                <img src="uniwork/Digital%20Marketing/8.png" alt="Poster 1">
                <img src="uniwork/Digital%20Marketing/7.png" alt="Poster 1">
                <img src="uniwork/Digital%20Marketing/3.jpg" alt="Poster 1">
                <img src="uniwork/Digital%20Marketing/1.jpg" alt="Poster 1">
            </div>
        </div>
    </div>
    <div class="projectUI" id="projectUI">
        <h2>UI Design</h2>
        <p>A university project where I had to redesign Europris' website to improve both the UI and UX.</p>
            <div class="project">
                <h3>Europris redesign</h3>
                <div class="scroll-gallery">
                    <img src="uniwork/UI%20Design/1.png" alt="Poster 1">
                    <img src="uniwork/UI%20Design/2.png" alt="Poster 1">
                    <img src="uniwork/UI%20Design/3.png" alt="Poster 1">
                    <img src="uniwork/UI%20Design/4.jpg" alt="Poster 1">
                    <img src="uniwork/UI%20Design/5.jpg" alt="Poster 1">
                    <img src="uniwork/UI%20Design/6.png" alt="Poster 1">
                    <img src="uniwork/UI%20Design/7.png" alt="Poster 1">
                    <img src="uniwork/UI%20Design/8.png" alt="Poster 1">
                </div>
            </div>
        </div>
        <div class="projectF" id="projectF">
            <h2>Freelance</h2>
            <p>A few freelance projects I've worked on in the past.</p>
            <div class="project">
                <div class="scroll-gallery">
                    <img src="uniwork/Freelance/1.png" alt="Poster 1">
                    <img src="uniwork/Freelance/2.png" alt="Poster 1">
                    <img src="uniwork/Freelance/3.png" alt="Poster 1">
                </div>
            </div>
        </div>

        </div>
    </div>

    <footer>
        <p>© 2025 Diogo Parcerias – Contact: diogo@decifrar.net +47 948 41 540</p>
    </footer>

    <script>
        document.querySelectorAll('.gallery, .scroll-gallery').forEach(gallery => {
            const images = gallery.querySelectorAll('img');

            images.forEach((img, index) => {
                img.addEventListener('click', () => {
                    const fullscreenDiv = document.createElement('div');
                    fullscreenDiv.classList.add('fullscreen');
                    fullscreenDiv.style.display = 'flex';

                    const fullscreenImg = document.createElement('img');
                    fullscreenImg.src = img.src;

                    const closeButton = document.createElement('span');
                    closeButton.textContent = '×';
                    closeButton.style.position = 'absolute';
                    closeButton.style.top = '10px';
                    closeButton.style.right = '20px';
                    closeButton.style.fontSize = '2rem';
                    closeButton.style.color = 'white';
                    closeButton.style.cursor = 'pointer';

                    const prevButton = document.createElement('span');
                    prevButton.textContent = '❮';
                    prevButton.style.position = 'absolute';
                    prevButton.style.left = '20px';
                    prevButton.style.top = '50%';
                    prevButton.style.transform = 'translateY(-50%)';
                    prevButton.style.fontSize = '2rem';
                    prevButton.style.color = 'white';
                    prevButton.style.cursor = 'pointer';

                    const nextButton = document.createElement('span');
                    nextButton.textContent = '❯';
                    nextButton.style.position = 'absolute';
                    nextButton.style.right = '20px';
                    nextButton.style.top = '50%';
                    nextButton.style.transform = 'translateY(-50%)';
                    nextButton.style.fontSize = '2rem';
                    nextButton.style.color = 'white';
                    nextButton.style.cursor = 'pointer';

                    fullscreenDiv.appendChild(fullscreenImg);
                    fullscreenDiv.appendChild(closeButton);
                    fullscreenDiv.appendChild(prevButton);
                    fullscreenDiv.appendChild(nextButton);
                    document.body.appendChild(fullscreenDiv);

                    const updateImage = (newIndex) => {
                        if (newIndex >= 0 && newIndex < images.length) {
                            fullscreenImg.src = images[newIndex].src;
                            currentIndex = newIndex;
                        }
                    };

                    let currentIndex = index;

                    prevButton.addEventListener('click', () => {
                        updateImage(currentIndex - 1);
                    });

                    nextButton.addEventListener('click', () => {
                        updateImage(currentIndex + 1);
                    });

                    closeButton.addEventListener('click', () => {
                        document.body.removeChild(fullscreenDiv);
                        document.removeEventListener('keydown', handleKeydown);
                    });

                    fullscreenDiv.addEventListener('click', (e) => {
                        if (e.target === fullscreenDiv) {
                            document.body.removeChild(fullscreenDiv);
                            document.removeEventListener('keydown', handleKeydown);
                        }
                    });

                    const handleKeydown = (e) => {
                        if (e.key === 'ArrowLeft') {
                            updateImage(currentIndex - 1);
                        } else if (e.key === 'ArrowRight') {
                            updateImage(currentIndex + 1);
                        } else if (e.key === 'Escape') {
                            document.body.removeChild(fullscreenDiv);
                            document.removeEventListener('keydown', handleKeydown);
                        }
                    };

                    document.addEventListener('keydown', handleKeydown);
                });
            });
        });

        document.querySelectorAll('nav button').forEach(button => {
            button.addEventListener('click', (event) => {
                const targetId = event.target.getAttribute('onclick').match(/\'(.*?)\'/)[1];
                const targetElement = document.getElementById(targetId);
                const offset = 90; // Adjust the offset as needed

                if (targetElement) {
                    const elementPosition = targetElement.getBoundingClientRect().top + window.scrollY;
                    window.scrollTo({
                        top: elementPosition - offset,
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>

