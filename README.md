<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cafe Fravé
    </title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #ffffff;
            color: #1a4314;
        }
        /* Custom styles for animations and states */
        .loading-spinner {
            border: 4px solid rgba(0, 0, 0, 0.1);
            border-left-color: #4caf50;
            border-radius: 50%;
            width: 24px;
            height: 24px;
            animation: spin 1s linear infinite;
        }
        @keyframes spin {
            to {
                transform: rotate(360deg);
            }
        }
        .font-montserrat {
            font-family: 'Montserrat', sans-serif;
        }

        /* Animations for elements appearing on scroll */
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease-out, transform 0.6s ease-out;
        }
        .fade-in.is-visible {
            opacity: 1;
            transform: translateY(0);
        }
        .fade-in-delay-1 { transition-delay: 0.1s; }
        .fade-in-delay-2 { transition-delay: 0.2s; }
        .fade-in-delay-3 { transition-delay: 0.3s; }

        .page {
            display: none;
            min-height: 100vh;
        }
        .page.active {
            display: block;
        }
    </style>
</head>
<body class="antialiased">

    <!-- Navbar -->
    <nav class="fixed top-0 inset-x-0 bg-white bg-opacity-90 backdrop-blur-md z-50 shadow-sm transition-all duration-300">
        <div class="max-w-6xl mx-auto px-6 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-3">
                <a href="#" class="text-2xl font-bold text-[#2e4d2e] hover:text-[#558b2f] transition-colors duration-300 page-link" data-page="home">
                    <img src="https://github.com/cafefrave/cafefrave.github.io/blob/main/503491142_17860619157422164_8610843937928964987_n.jpg?raw=true" alt="Cafe Fravé Logo" class="w-12 h-12 rounded-full shadow-lg transition-transform hover:scale-110">
                </a>
                <a href="#" class="text-2xl font-bold font-montserrat text-[#1a4314] page-link" data-page="home">Cafe Fravé</a>
            </div>
            <div class="flex space-x-4 md:space-x-8 items-center">
                <a href="#about" class="text-lg text-[#1a4314] hover:text-[#4caf50] transition duration-300 page-link" data-page="home" data-target="#about">About Us</a>
                <a href="#" class="text-lg text-[#1a4314] hover:text-[#4caf50] transition duration-300 page-link" data-page="menu-page">Menu</a>
                <a href="#" class="text-lg text-[#1a4314] hover:text-[#4caf50] transition duration-300 page-link" data-page="contact-page">Contact</a>
            </div>
        </div>
    </nav>
    
    <!-- Home Page -->
    <div id="home" class="page active">
        <!-- Hero Section -->
        <section class="relative h-[60vh] md:h-[80vh] bg-cover bg-center flex items-center justify-center p-4 text-center text-white" style="background-image: url('https://lh3.googleusercontent.com/gps-cs-s/AC9h4noJau0-ApCljbmK3aRm1rEvZog_q5oUPNdbGCMQi_JeglKV4Zg6ZrZc242lc107Z2_XXLa-e_eKJ3Fb-eqTrxKNsuzaS9St9jhzHvieQ-3i2YjkU3S8a_rx4AEKZdxCz6RroFSkOKqarmxS=s1360-w1360-h1020-rw');">
            <div class="absolute inset-0 bg-black opacity-0"></div>
            <div class="z-10 w-full h-full">
                <!-- Content here can be added if needed, or left empty to just show the background -->
            </div>
        </section>
        
        <!-- About Us Section -->
        <section id="about" class="py-16 px-4 md:px-8 bg-white">
            <div class="max-w-6xl mx-auto text-center">
                <h2 class="text-3xl md:text-4xl font-bold mb-4 text-[#1a4314] font-montserrat fade-in">About Us</h2>
                <div class="grid md:grid-cols-2 gap-12 items-center">
                    <div class="flex flex-col text-left space-y-4 fade-in fade-in-delay-1">
                        <p class="text-lg text-gray-700 leading-relaxed">
                            BE CONSCIOUSLY CAFFEINATED
                        </p>
                        <p class="text-lg text-gray-700 leading-relaxed">
                            At Fravé, we believe food is more than just nourishment — it's a way of living with intention. Our menu is built around the idea of unprocessed, clean eating, everything is made from scratch, with ingredients you can trust.
                        </p>
                        <p class="text-lg text-gray-700 leading-relaxed">
                            We skip refined sugar — using only natural sweeteners like jaggery, dates, and raw cane sugar in everything we create.
                        </p>
                    </div>
                    <div class="relative w-full h-80 fade-in fade-in-delay-2">
                        <video autoplay loop muted playsinline class="absolute inset-0 w-full h-full object-cover rounded-lg shadow-xl">
                            <source src="https://drive.google.com/file/d/19HDntbCoj5ypFKYalrhbaTRxG3GqSHMw/preview" type="video/mp4">
                            Your browser does not support the video tag.
                        </video>
                    </div>
                </div>
                <p class="text-lg text-gray-700 leading-relaxed mt-8 fade-in fade-in-delay-3">
                    At Fravé, we proudly embrace a 90% plant-based philosophy. Thank you for being part of this journey toward better, more conscious living.
                </p>
            </div>
        </section>
    </div>

    <!-- Menu Page -->
    <div id="menu-page" class="page">
        <!-- Menu Section -->
        <section id="menu" class="bg-gray-100 py-16 px-4 md:px-8">
            <div class="max-w-6xl mx-auto text-center">
                <h2 class="text-3xl md:text-4xl font-bold mb-8 text-[#1a4314] font-montserrat fade-in">Our Menu</h2>
    
                <!-- Smoothies & Frappes Section -->
                <h3 class="text-2xl font-semibold mb-4 text-[#1a4314] border-b-2 border-dashed border-[#4caf50] inline-block pb-1 font-montserrat fade-in fade-in-delay-1">Smoothies & Frappes</h3>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mb-12 mt-4">
                    <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105 fade-in fade-in-delay-2">
                        <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Smoothie" alt="Pink Rumba Smoothie" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                        <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Pink Rumba Smoothie</h4>
                        <p class="text-gray-600">Pink Guava | Strawberries | Basil seeds I Coconut milk | Raw Cane Sugar</p>
                        <span class="block mt-4 text-xl font-bold text-[#4caf50]">Regular ₹270 | Bowl ₹320</span>
                    </div>
                    <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105 fade-in fade-in-delay-3">
                        <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Smoothie" alt="Mocha Brew Smoothie" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                        <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Mocha Brew Smoothie</h4>
                        <p class="text-gray-600"> vanilla | Dates | Banana | 100% Cacao | Peanut Butter| Almond milk</p>
                        <span class="block mt-4 text-xl font-bold text-[#4caf50]">Regular ₹290 | Bowl ₹350</span>
                    </div>
                    <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105 fade-in fade-in-delay-4">
                        <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Smoothie" alt="Berry Groove Smoothie" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                        <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Berry Groove Smoothie </h4>
                        <p class="text-gray-600">Mixed berries, yogurt, and granola topped with fresh fruit.</p>
                        <span class="block mt-4 text-xl font-bold text-[#4caf50]">Regular ₹280 | Bowl ₹340</span>
                    </div>
                    <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105 fade-in fade-in-delay-5">
                        <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Frappe" alt="Frappe Fravé" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                        <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Frappe Fravé</h4>
                        <p class="text-gray-600">Homemade Almond Butter | Espresso | Walnuts | House Almond Milk | Vanilla Gelato</p>
                        <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹220</span>
                    </div>
                    <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105 fade-in fade-in-delay-6">
                        <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Frappe" alt="Mocha Berry Fravé" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                        <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Mocha Berry Fravé</h4>
                        <p class="text-gray-600">Espresso | Strawberries | Raspberries | Vanilla Gelato | Milk | 100% Cacao</p>
                        <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹240</span>
                    </div>
                    <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105 fade-in fade-in-delay-7">
                        <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Hot+Chocolate" alt="Cinnamon Drift Hot Chocolate" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                        <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Cinnamon Drift Hot Chocolate</h4>
                        <p class="text-gray-600">100% Cacao | Milk Cinnamon | Nutmeg Organic Jaggery</p>
                        <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹199</span>
                    </div>
                </div>

                <!-- Pastas Section -->
                <h3 class="text-2xl font-semibold mb-4 text-[#1a4314] border-b-2 border-dashed border-[#4caf50] inline-block pb-1 font-montserrat fade-in fade-in-delay-8">Pastas</h3>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mt-4">
                    <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105 fade-in fade-in-delay-9">
                        <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Pasta" alt="Red Ember Penne" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                        <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Red Ember Penne</h4>
                        <p class="text-gray-600">Penne Pasta | Inhouse Marinara Sauce | Zucchini | Bell Peppers | Mushrooms</p>
                        <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹320</span>
                    </div>
                    <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105 fade-in fade-in-delay-10">
                        <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Pasta" alt="White Viel Pasta" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                        <h4 class="font-bold text-xl mb-2 text-[#1a4314]">White Viel Pasta</h4>
                        <p class="text-gray-600">Penne pasta | Béchamel Sauce | Mushrooms | Parmesan | Truffle Oil</p>
                        <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹299</span>
                    </div>
                    <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105 fade-in fade-in-delay-11">
                        <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Pasta" alt="SPAGHETTI AGLIO E OLIO" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                        <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Spaghetti Aglio E Olio</h4>
                        <p class="text-gray-600">Spaghetti Pasta | Olive oil | Garlic | Parsley | Herbs</p>
                        <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹289</span>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Contact Page -->
    <div id="contact-page" class="page">
        <!-- Contact Section -->
        <section id="contact" class="bg-white py-16 px-4 md:px-8">
            <div class="max-w-4xl mx-auto text-center">
                <h2 class="text-3xl md:text-4xl font-bold mb-8 text-[#1a4314] font-montserrat fade-in">Get In Touch</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                    <!-- Contact Form -->
                    <div class="bg-gray-100 rounded-lg shadow-lg p-8 fade-in fade-in-delay-1">
                        <form id="contactForm" class="flex flex-col gap-4">
                            <input type="text" id="name" placeholder="Your Name" class="p-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-[#4caf50]" required>
                            <input type="email" id="email" placeholder="Your Email" class="p-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-[#4caf50]" required>
                            <textarea id="message" placeholder="Your Message" rows="4" class="p-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-[#4caf50]" required></textarea>
                            <button type="submit" id="submitBtn" class="bg-[#1a4314] hover:bg-[#122e0e] text-white font-semibold py-3 px-6 rounded-lg transition duration-300 flex items-center justify-center">
                                Send Message
                            </button>
                        </form>
                        <div id="formMessage" class="mt-4 text-center hidden"></div>
                    </div>
    
                    <!-- Cafe Info -->
                    <div class="bg-gray-100 rounded-lg shadow-lg p-8 flex flex-col justify-center fade-in fade-in-delay-2">
                        <h3 class="text-xl font-bold mb-4 text-[#1a4314]">Visit Us</h3>
                        <a href="https://maps.app.goo.gl/uWvz1gaGdxPxBPr4A" class="hover:text-[#4caf50] transition duration-300">258, Survey Nagar, Near Kalimata Mandir, Nagpur 440022</a>
                            <p class="text-lg text-gray-700 mb-2"><strong>Phone:</strong> +91 8087720122</p>
                            <p class="text-lg text-gray-700 mb-4"><strong>Email:</strong> cafe.frave@gmail.com</p>
                            <h3 class="text-2xl font-bold mb-4 mt-6">Hours</h3>
                            <p class="text-lg text-gray-700">Dine-In (12pm -10pm), Tuesdays Closed</p>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Footer -->
    <footer class="bg-[#1a4314] text-white py-8 px-4 md:px-8 text-center">
        <div class="max-w-6xl mx-auto">
            <p>&copy; 2025 Cafe Fravé. All Rights Reserved.</p>
            <div class="mt-4 flex justify-center space-x-4">
                <a href="https://www.instagram.com/frave.cafe/" class="hover:text-[#4caf50] transition duration-300">Instagram</a>
                <a href="https://g.co/kgs/2wztXyN" class="hover:text-[#4caf50] transition duration-300">Fravé on Google</a>
                <a href="https://zomato.onelink.me/xqzv/lgh8pm27" class="hover:text-[#4caf50] transition duration-300">Zomato</a>
                <a href="https://www.swiggy.com/city/nagpur/frave-pratap-nagar-rest1095085?source=sharing" class="hover:text-[#4caf50] transition duration-300">Swiggy</a>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling for all internal anchor links
        document.querySelectorAll('a[href^="#"].scroll-link').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();

                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);

                if (targetElement) {
                    targetElement.scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Client-side routing for "pages"
        document.querySelectorAll('.page-link').forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                const pageId = this.getAttribute('data-page');
                const targetId = this.getAttribute('data-target');

                // Hide all pages
                document.querySelectorAll('.page').forEach(page => {
                    page.classList.remove('active');
                });

                // Show the target page
                document.getElementById(pageId).classList.add('active');

                // Scroll to the top of the page unless there's a specific target
                if (targetId) {
                    const targetElement = document.querySelector(targetId);
                    if (targetElement) {
                        const navbarHeight = document.querySelector('nav').offsetHeight;
                        setTimeout(() => {
                           window.scrollTo({
                                top: targetElement.offsetTop - navbarHeight,
                                behavior: 'smooth'
                            });
                        }, 50); // Small delay to allow the page to become active
                    }
                } else {
                    window.scrollTo({ top: 0, behavior: 'smooth' });
                }
            });
        });


        // Add scroll-based animations
        const observerOptions = {
            root: null,
            rootMargin: '0px',
            threshold: 0.2 // Trigger when 20% of the element is visible
        };

        const observer = new IntersectionObserver((entries, observer) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('is-visible');
                    observer.unobserve(entry.target);
                }
            });
        }, observerOptions);

        const animatedElements = document.querySelectorAll('.fade-in');
        animatedElements.forEach(el => observer.observe(el));


        document.getElementById('contactForm').addEventListener('submit', async function(event) {
            event.preventDefault();

            const formMessage = document.getElementById('formMessage');
            const submitBtn = document.getElementById('submitBtn');

            // Show a loading state
            submitBtn.innerHTML = '<div class="loading-spinner"></div>';
            submitBtn.disabled = true;

            const formData = {
                name: document.getElementById('name').value,
                email: document.getElementById('email').value,
                message: document.getElementById('message').value
            };

            try {
                // Simulate a network request. In a real-world scenario, you would replace this with an actual API endpoint.
                await new Promise(resolve => setTimeout(resolve, 2000));
                
                // For demonstration, we'll assume the submission was successful.
                const response = { success: true }; 

                if (response.success) {
                    formMessage.textContent = 'Thank you for your message! We will get back to you shortly.';
                    formMessage.classList.remove('hidden', 'text-red-600');
                    formMessage.classList.add('text-green-600', 'font-semibold');
                    this.reset();
                } else {
                    throw new Error('Form submission failed.');
                }
            } catch (error) {
                console.error('Error submitting form:', error);
                formMessage.textContent = 'Oops! Something went wrong. Please try again.';
                formMessage.classList.remove('hidden', 'text-green-600');
                formMessage.classList.add('text-red-600', 'font-semibold');
            } finally {
                // Reset button to original state
                submitBtn.innerHTML = 'Send Message';
                submitBtn.disabled = false;
                
                // Hide message after a few seconds
                setTimeout(() => {
                    formMessage.classList.add('hidden');
                }, 5000);
            }
        });
    </script>

</body>
</html>
