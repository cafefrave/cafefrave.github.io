<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cafe Fravé</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #f8fcf5;
            color: #2e4d2e;
        }
        .loading-spinner {
            border: 4px solid rgba(0, 0, 0, 0.1);
            border-left-color: #558b2f;
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
    </style>
</head>
<body class="antialiased">

    <!-- Navbar -->
    <nav class="fixed top-0 inset-x-0 bg-white bg-opacity-90 backdrop-blur-md z-50 shadow-sm transition-all duration-300">
        <div class="container mx-auto px-6 py-3 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold text-[#2e4d2e] hover:text-[#558b2f] transition-colors duration-300">Cafe Fravé</a>
            <div class="hidden md:flex space-x-8 items-center">
                <a href="#about" class="text-[#2e4d2e] hover:text-[#558b2f] transition-colors duration-300">About Us</a>
                <a href="#menu" class="text-[#2e4d2e] hover:text-[#558b2f] transition-colors duration-300">Menu</a>
                <a href="#contact" class="text-[#2e4d2e] hover:text-[#558b2f] transition-colors duration-300">Contact</a>
                <img src="503491142_17860619157422164_8610843937928964987_n.jpg" alt="Cafe Fravé Logo" class="w-10 h-10 rounded-full shadow-lg ml-8">
            </div>
            <!-- Mobile Menu Button -->
            <button id="mobile-menu-btn" class="md:hidden text-[#2e4d2e]">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                </svg>
            </button>
        </div>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white bg-opacity-90 backdrop-blur-md">
            <a href="#about" class="block py-2 px-6 hover:bg-gray-100 transition-colors duration-300">About Us</a>
            <a href="#menu" class="block py-2 px-6 hover:bg-gray-100 transition-colors duration-300">Menu</a>
            <a href="#contact" class="block py-2 px-6 hover:bg-gray-100 transition-colors duration-300">Contact</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative h-screen flex items-center justify-center p-4">
        <div class="absolute inset-0 bg-cover bg-center" style="background-image: url('https://lh3.googleusercontent.com/gps-cs-s/AC9h4noJau0-ApCljbmK3aRm1rEvZog_q5oUPNdbGCMQi_JeglKV4Zg6ZrZc242lc107Z2_XXLa-e_eKJ3Fb-eqTrxKNsuzaS9St9jhzHvieQ-3i2YjkU3S8a_rx4AEKZdxCz6RroFSkOKqarmxS=s1360-w1360-h1020-rw');"></div>
        <div class="absolute inset-0 bg-black opacity-30"></div>
        <div class="z-10 text-center text-white">
            <h1 class="text-5xl md:text-7xl font-bold mb-4 animate-fade-in-up">BE CONSCIOUSLY CAFFEINATED</h1>
            <p class="text-xl md:text-2xl mb-8 animate-fade-in-up delay-150">At Fravé, we believe food is more than just nourishment.</p>
            <a href="#menu" id="hero-menu-btn" class="inline-block px-8 py-3 bg-white text-[#2e4d2e] font-semibold rounded-full shadow-lg hover:bg-gray-100 transition-colors duration-300 animate-fade-in-up delay-300">Explore Our Menu</a>
        </div>
    </section>

    <!-- About Us Section -->
    <section id="about" class="py-20 bg-white px-6">
        <div class="max-w-6xl mx-auto flex flex-col md:flex-row items-center gap-12">
            <div class="md:w-1/2">
                <img src="https://placehold.co/600x400/b8d9a4/2e4d2e?text=Our+Philosophy" alt="About Us" class="rounded-lg shadow-xl">
            </div>
            <div class="md:w-1/2 text-center md:text-left">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Our Philosophy</h2>
                <p class="text-lg text-gray-700 leading-relaxed mb-4">
                    At Fravé, we believe food is more than just nourishment — it's a way of living with intention. Our menu is built around the idea of unprocessed, clean eating, everything is made from scratch, with ingredients you can trust.
                </p>
                
                <p class="text-lg text-gray-700 leading-relaxed mt-4">
                    At Fravé, we proudly embrace a 90% plant-based philosophy, our heart stays rooted in creating meals that are mindful, balanced, and kind — both to you and to the planet. Thank you for being part of this journey toward better, more conscious living.
                </p>
            </div>
        </div>
    </section>

    <!-- Menu Section -->
    <section id="menu" class="py-20 bg-[#f8fcf5] px-6">
        <div class="max-w-6xl mx-auto text-center">
            <h2 class="text-4xl font-bold mb-12">Our Menu</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Smoothies & Juices Section -->
                <div class="bg-white rounded-xl shadow-lg p-8">
                    <h3 class="text-2xl font-bold mb-6 border-b-2 border-dashed border-[#a3c7a3] inline-block pb-2">Smoothies </h3>
                    <ul class="text-left space-y-4">
                        <li class="flex justify-between items-center">
                            <span>Pink Rumba Smoothie</span>
                            <span class="font-bold text-[#558b2f]">Regular ₹270 | Bowl ₹320</span>
                        </li>
                        <li class="flex justify-between items-center">
                            <span>Berry Groove Smoothie</span>
                            <span class="font-bold text-[#558b2f]">Regular ₹280 | Bowl ₹340</span>
                        </li>
                        
                    </ul>
                </div>

                <!-- Pastas Section -->
                <div class="bg-white rounded-xl shadow-lg p-8">
                    <h3 class="text-2xl font-bold mb-6 border-b-2 border-dashed border-[#a3c7a3] inline-block pb-2">Pastas and Frappes</h3>
                    <ul class="text-left space-y-4">
                        <li class="flex justify-between items-center">
                            <span>Red Ember Penne</span>
                            <span class="font-bold text-[#558b2f]">₹320</span>
                        </li>
                        <li class="flex justify-between items-center">
                            <span>White Viel Pasta</span>
                            <span class="font-bold text-[#558b2f]">₹299</span>
                        <li class="flex justify-between items-center">
                            <span>Frappe Fravé</span>
                            <span class="font-bold text-[#558b2f]">₹220</span>
                        </li>
                        <li class="flex justify-between items-center">
                            <span>Mocha Berry Fravé</span>
                            <span class="font-bold text-[#558b2f]">₹240</span>
                        </li>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-[#f8fcf5] px-6">
        <div class="max-w-6xl mx-auto text-center">
            <h2 class="text-4xl font-bold mb-6">Get In Touch</h2>
            <div class="flex flex-col md:flex-row justify-center items-center gap-12">
                <div class="md:w-1/2">
                    <form id="contactForm" class="flex flex-col gap-6 p-8 bg-white rounded-xl shadow-lg">
                        <input type="text" id="name" placeholder="Name" class="p-4 border border-[#e0e0e0] rounded-lg focus:outline-none focus:ring-2 focus:ring-[#a3c7a3]" required>
                        <input type="email" id="email" placeholder="Email" class="p-4 border border-[#e0e0e0] rounded-lg focus:outline-none focus:ring-2 focus:ring-[#a3c7a3]" required>
                        <textarea id="message" placeholder="Message" rows="5" class="p-4 border border-[#e0e0e0] rounded-lg focus:outline-none focus:ring-2 focus:ring-[#a3c7a3]" required></textarea>
                        <button type="submit" id="submitBtn" class="px-6 py-3 bg-[#558b2f] text-white font-bold rounded-lg hover:bg-[#2e4d2e] transition-colors duration-300">Send Message</button>
                    </form>
                    <div id="formMessage" class="mt-4 text-center hidden"></div>
                </div>
                <div class="md:w-1/2">
                    <div class="p-8 bg-white rounded-xl shadow-lg text-left">
                        <h3 class="text-2xl font-bold mb-4">Visit Us</h3>
                        <a href="https://maps.app.goo.gl/uWvz1gaGdxPxBPr4A" class="hover:text-[#4caf50] transition duration-300">258, Survey Nagar, Near Kalimata Mandir, Nagpur 440022</a>
                        <p class="text-lg text-gray-700 mb-2"><strong>Phone:</strong> +91 8087720122</p>
                        <p class="text-lg text-gray-700 mb-4"><strong>Email:</strong> cafe.frave@gmail.com</p>
                        <h3 class="text-2xl font-bold mb-4 mt-6">Hours</h3>
                        <p class="text-lg text-gray-700">Dine-In (12pm -10pm), Tuesdays Closed</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

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
        document.getElementById('mobile-menu-btn').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });

        // Smooth scroll for all nav links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    targetElement.scrollIntoView({ behavior: 'smooth' });
                }
            });
        });

        // Contact form submission logic
        document.getElementById('contactForm').addEventListener('submit', async function(event) {
            event.preventDefault();
            const formMessage = document.getElementById('formMessage');
            const submitBtn = document.getElementById('submitBtn');

            submitBtn.innerHTML = '<div class="loading-spinner"></div>';
            submitBtn.disabled = true;

            const formData = {
                name: document.getElementById('name').value,
                email: document.getElementById('email').value,
                message: document.getElementById('message').value
            };

            try {
                // In a real-world scenario, you would send formData to a backend endpoint here.
                console.log('Form Data:', formData);
                await new Promise(resolve => setTimeout(resolve, 2000));
                
                const response = { success: true }; 

                if (response.success) {
                    formMessage.textContent = 'Thank you for your message! We will get back to you shortly.';
                    formMessage.classList.remove('hidden', 'text-red-600');
                    formMessage.classList.add('text-[#558b2f]', 'font-semibold');
                    this.reset();
                } else {
                    throw new Error('Form submission failed.');
                }
            } catch (error) {
                console.error('Error submitting form:', error);
                formMessage.textContent = 'Oops! Something went wrong. Please try again.';
                formMessage.classList.remove('hidden', 'text-[#558b2f]');
                formMessage.classList.add('text-red-600', 'font-semibold');
            } finally {
                submitBtn.innerHTML = 'Send Message';
                submitBtn.disabled = false;
                setTimeout(() => {
                    formMessage.classList.add('hidden');
                }, 5000);
            }
        });
    </script>

</body>
</html>
