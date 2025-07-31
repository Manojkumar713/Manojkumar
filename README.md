<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>John Doe - Professional Portfolio</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts: Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Custom Styles -->
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #111827; /* Dark background */
            color: #E5E7EB; /* Light text */
        }
        /* Style for the reveal-on-scroll animation */
        .reveal {
            position: relative;
            transform: translateY(100px);
            opacity: 0;
            transition: all 1s ease;
        }
        .reveal.active {
            transform: translateY(0px);
            opacity: 1;
        }
    </style>
</head>
<body class="antialiased">

    <!-- Header & Navigation -->
    <header class="bg-gray-900/80 backdrop-blur-sm sticky top-0 z-50">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold text-white">JD.</a>
            <div class="hidden md:flex space-x-6 items-center">
                <a href="#about" class="text-gray-300 hover:text-cyan-400 transition duration-300">About</a>
                <a href="#projects" class="text-gray-300 hover:text-cyan-400 transition duration-300">Projects</a>
                <a href="#skills" class="text-gray-300 hover:text-cyan-400 transition duration-300">Skills</a>
                <a href="#contact" class="bg-cyan-500 hover:bg-cyan-600 text-white font-semibold px-4 py-2 rounded-lg transition duration-300">Contact Me</a>
            </div>
            <!-- Mobile Menu Button -->
            <button id="mobile-menu-button" class="md:hidden text-white">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                </svg>
            </button>
        </nav>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden px-6 pb-4 space-y-2">
            <a href="#about" class="block text-gray-300 hover:text-cyan-400 transition duration-300">About</a>
            <a href="#projects" class="block text-gray-300 hover:text-cyan-400 transition duration-300">Projects</a>
            <a href="#skills" class="block text-gray-300 hover:text-cyan-400 transition duration-300">Skills</a>
            <a href="#contact" class="block bg-cyan-500 hover:bg-cyan-600 text-white font-semibold px-4 py-2 rounded-lg transition duration-300 mt-2 text-center">Contact Me</a>
        </div>
    </header>

    <main class="container mx-auto px-6">

        <!-- Hero Section -->
        <section id="hero" class="min-h-screen flex items-center">
            <div class="text-center md:text-left w-full">
                <h1 class="text-4xl md:text-6xl font-bold text-white leading-tight mb-4">
                    Hi, I'm John Doe
                </h1>
                <p class="text-xl md:text-2xl text-cyan-400 font-semibold mb-8">
                    A Passionate Web Developer & UI/UX Enthusiast
                </p>
                <p class="max-w-2xl mx-auto md:mx-0 text-gray-300 mb-8">
                    I build beautiful, responsive, and user-friendly websites and applications. Turning complex problems into elegant digital solutions is my specialty.
                </p>
                <a href="#projects" class="bg-transparent border-2 border-cyan-400 text-cyan-400 hover:bg-cyan-400 hover:text-gray-900 font-bold py-3 px-8 rounded-lg transition duration-300">
                    View My Work
                </a>
            </div>
        </section>

        <!-- About Section -->
        <section id="about" class="py-20 reveal">
            <h2 class="text-3xl font-bold text-center text-white mb-12">About Me</h2>
            <div class="flex flex-col md:flex-row items-center gap-10">
                <div class="w-full md:w-1/3">
                    <img src="https://placehold.co/400x400/1F2937/E5E7EB?text=Your+Photo" 
                         onerror="this.onerror=null;this.src='https://placehold.co/400x400/1F2937/E5E7EB?text=Image+Error';"
                         alt="A portrait of John Doe" class="rounded-full shadow-lg mx-auto">
                </div>
                <div class="w-full md:w-2/3 text-center md:text-left">
                    <h3 class="text-2xl font-semibold text-cyan-400 mb-4">Who I Am</h3>
                    <p class="text-gray-300 leading-relaxed">
                        Hello! I'm John, a developer based in New York. My journey into web development started years ago with a fascination for how things work on the internet. Today, I have a deep passion for creating seamless digital experiences. I specialize in front-end development but am also proficient in back-end technologies. When I'm not coding, I enjoy hiking, photography, and exploring new coffee shops.
                    </p>
                </div>
            </div>
        </section>

        <!-- Projects Section -->
        <section id="projects" class="py-20 reveal">
            <h2 class="text-3xl font-bold text-center text-white mb-12">My Projects</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <!-- Project Card 1 -->
                <div class="bg-gray-800 rounded-lg overflow-hidden shadow-lg transform hover:-translate-y-2 transition duration-300">
                    <img src="https://placehold.co/600x400/3B82F6/FFFFFF?text=Project+1" 
                         onerror="this.onerror=null;this.src='https://placehold.co/600x400/3B82F6/FFFFFF?text=Image+Error';"
                         alt="Project 1 Screenshot" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-white mb-2">E-commerce Platform</h3>
                        <p class="text-gray-400 mb-4">A fully-featured e-commerce site built with React, Node.js, and Stripe for payments.</p>
                        <a href="#" class="text-cyan-400 hover:text-cyan-300 font-semibold">View Details &rarr;</a>
                    </div>
                </div>

                <!-- Project Card 2 -->
                <div class="bg-gray-800 rounded-lg overflow-hidden shadow-lg transform hover:-translate-y-2 transition duration-300">
                    <img src="https://placehold.co/600x400/10B981/FFFFFF?text=Project+2" 
                         onerror="this.onerror=null;this.src='https://placehold.co/600x400/10B981/FFFFFF?text=Image+Error';"
                         alt="Project 2 Screenshot" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-white mb-2">Task Management App</h3>
                        <p class="text-gray-400 mb-4">A sleek and intuitive task manager to boost productivity, built with Vue.js and Firebase.</p>
                        <a href="#" class="text-cyan-400 hover:text-cyan-300 font-semibold">View Details &rarr;</a>
                    </div>
                </div>

                <!-- Project Card 3 -->
                <div class="bg-gray-800 rounded-lg overflow-hidden shadow-lg transform hover:-translate-y-2 transition duration-300">
                    <img src="https://placehold.co/600x400/F59E0B/FFFFFF?text=Project+3" 
                         onerror="this.onerror=null;this.src='https://placehold.co/600x400/F59E0B/FFFFFF?text=Image+Error';"
                         alt="Project 3 Screenshot" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-white mb-2">Portfolio Website Template</h3>
                        <p class="text-gray-400 mb-4">A responsive and customizable portfolio template created with HTML, CSS, and JavaScript.</p>
                        <a href="#" class="text-cyan-400 hover:text-cyan-300 font-semibold">View Details &rarr;</a>
                    </div>
                </div>

            </div>
        </section>

        <!-- Skills Section -->
        <section id="skills" class="py-20 reveal">
            <h2 class="text-3xl font-bold text-center text-white mb-12">My Skills</h2>
            <div class="max-w-4xl mx-auto">
                <div class="flex flex-wrap justify-center gap-4">
                    <span class="bg-gray-700 text-gray-200 text-lg font-semibold px-5 py-2 rounded-full">HTML5</span>
                    <span class="bg-gray-700 text-gray-200 text-lg font-semibold px-5 py-2 rounded-full">CSS3 & Tailwind</span>
                    <span class="bg-gray-700 text-gray-200 text-lg font-semibold px-5 py-2 rounded-full">JavaScript (ES6+)</span>
                    <span class="bg-gray-700 text-gray-200 text-lg font-semibold px-5 py-2 rounded-full">React</span>
                    <span class="bg-gray-700 text-gray-200 text-lg font-semibold px-5 py-2 rounded-full">Vue.js</span>
                    <span class="bg-gray-700 text-gray-200 text-lg font-semibold px-5 py-2 rounded-full">Node.js</span>
                    <span class="bg-gray-700 text-gray-200 text-lg font-semibold px-5 py-2 rounded-full">Firebase</span>
                    <span class="bg-gray-700 text-gray-200 text-lg font-semibold px-5 py-2 rounded-full">Git & GitHub</span>
                    <span class="bg-gray-700 text-gray-200 text-lg font-semibold px-5 py-2 rounded-full">UI/UX Design</span>
                    <span class="bg-gray-700 text-gray-200 text-lg font-semibold px-5 py-2 rounded-full">Figma</span>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="py-20 reveal">
            <h2 class="text-3xl font-bold text-center text-white mb-4">Get In Touch</h2>
            <p class="text-center text-gray-400 max-w-xl mx-auto mb-12">
                I'm currently available for freelance work and open to new opportunities. If you have a project in mind or just want to say hello, feel free to reach out!
            </p>
            <div class="text-center">
                <a href="mailto:your.email@example.com" class="bg-cyan-500 hover:bg-cyan-600 text-white font-bold py-4 px-8 rounded-lg transition duration-300 text-lg">
                    Say Hello
                </a>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 border-t border-gray-800">
        <div class="container mx-auto px-6 py-8 text-center text-gray-400">
            <div class="flex justify-center space-x-6 mb-4">
                <a href="#" class="hover:text-cyan-400 transition duration-300">GitHub</a>
                <a href="#" class="hover:text-cyan-400 transition duration-300">LinkedIn</a>
                <a href="#" class="hover:text-cyan-400 transition duration-300">Twitter</a>
            </div>
            <p>&copy; 2025 John Doe. All Rights Reserved.</p>
        </div>
    </footer>

    <!-- Scroll-to-top Button -->
    <button id="to-top-button" title="Go To Top"
        class="hidden fixed bottom-8 right-8 p-3 rounded-full bg-cyan-500 text-white hover:bg-cyan-600 transition-opacity duration-300 shadow-lg">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 15l7-7 7 7" />
        </svg>
    </button>

    <!-- JavaScript -->
    <script>
        document.addEventListener('DOMContentLoaded', function () {
            
            // --- Mobile Menu Toggle ---
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });

            // --- Reveal on Scroll Animation ---
            function reveal() {
                const reveals = document.querySelectorAll('.reveal');
                for (let i = 0; i < reveals.length; i++) {
                    const windowHeight = window.innerHeight;
                    const elementTop = reveals[i].getBoundingClientRect().top;
                    const elementVisible = 150; // Distance from bottom of viewport to trigger animation

                    if (elementTop < windowHeight - elementVisible) {
                        reveals[i].classList.add('active');
                    } else {
                        reveals[i].classList.remove('active');
                    }
                }
            }
            window.addEventListener('scroll', reveal);
            // Initial check
            reveal();

            // --- Scroll-to-Top Button ---
            const toTopButton = document.getElementById('to-top-button');
            
            window.onscroll = function () {
                if (document.body.scrollTop > 200 || document.documentElement.scrollTop > 200) {
                    toTopButton.classList.remove('hidden');
                } else {
                    toTopButton.classList.add('hidden');
                }
            };

            toTopButton.onclick = function () {
                window.scrollTo({ top: 0, behavior: 'smooth' });
            };

        });
    </script>

</body>
</html>
