<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cafe Fravé
    </title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f9eb;
            color: #1a4314;
            scroll-behavior: smooth;
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
    </style>
</head>
<body class="antialiased">

    <!-- Hero Section -->
    <section class="relative h-[60vh] md:h-[80vh] bg-cover bg-center flex items-center justify-center p-4 text-center text-white" style="background-image: url('https://placehold.co/1200x800/2f643e/ffffff?text=Fresh+and+Healthy');">
        <div class="absolute inset-0 bg-black opacity-60"></div>
        <!-- Adjusted transform to move the content down -->
        <div class="z-10 max-w-2xl">
            <!-- Increased margin to create more space -->
            <h1 class="text-4xl md:text-6xl font-bold mb-40">Cafe Fravé</h1>
            <a href="#menu" class="bg-[#4caf50] hover:bg-[#388e3c] text-white font-semibold py-3 px-8 rounded-full shadow-lg transition duration-300">Explore Our Menu</a>
        </div>
    </section>
    
    <!-- Fresh & Healthy Section -->
    <section id="fresh-healthy" class="py-16 px-4 md:px-8">
        <div class="max-w-6xl mx-auto text-center">
            <h2 class="text-3xl md:text-4xl font-bold mb-4 text-[#1a4314]">About Us</h2>
            <p class="text-lg text-gray-700 leading-relaxed mb-6">
                BE CONSCIOUSLY CAFFEINATED
            </p>
            <p class="text-lg text-gray-700 leading-relaxed mb-6">
                At Fravé, we believe food is more than just nourishment — it's a way of living with intention.
            </p>
            <p class="text-lg text-gray-700 leading-relaxed mb-6">
                Our menu is built around the idea of unprocessed, clean eating, offering meal-replacement smoothie bowls, cold brews, plant-based lattes & frappes, freshly made pastas tossed in small-batch sauces — everything is made from scratch, with ingredients you can trust.
            </p>
            <p class="text-lg text-gray-700 leading-relaxed mb-6">
                Every element at Fravé is thoughtfully made:
                <ul class="list-disc list-inside mt-2 text-left mx-auto max-w-2xl">
                    <li>Nut butters, milks, syrups, and sauces are crafted in-house, ensuring pure, honest flavors.</li>
                    <li>We skip refined sugar — using only natural sweeteners like jaggery, dates, and raw cane sugar in everything we create.</li>
                </ul>
            </p>
            <p class="text-lg text-gray-700 leading-relaxed">
            .
            </p>
            <p class="text-lg text-gray-700 leading-relaxed">
                At Fravé, we proudly embrace a 90% plant-based philosophy. While a few ingredients may step outside the plant-based line, our heart stays rooted in creating meals that are mindful, balanced, and kind — both to you and to the planet. Thank you for being part of this journey toward better, more conscious living.
            </p>
        </div>
    </section>

    <!-- Menu Section -->
    <section id="menu" class="bg-[#eaf4e5] py-16 px-4 md:px-8">
        <div class="max-w-6xl mx-auto text-center">
            <h2 class="text-3xl md:text-4xl font-bold mb-8 text-[#1a4314]">Our Menu</h2>

            <!-- Smoothies & Frappes Section -->
            <h3 class="text-2xl font-semibold mb-4 text-[#1a4314] border-b-2 border-dashed border-[#4caf50] inline-block pb-1">Smoothies & Frappes</h3>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mb-12 mt-4">
                <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105">
                    <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Smoothie" alt="Green Smoothie" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                    <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Pink Rumba Smoothie</h4>
                    <p class="text-gray-600">Pink Guava | Strawberries | Basil seeds I
 Coconut milk | Raw Cane Sugar</p>
                    <span class="block mt-4 text-xl font-bold text-[#4caf50]">Regular ₹270 | Bowl ₹320</span>
                </div>
		<div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105">
                    <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Smoothie" alt="Green Smoothie" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                    <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Mocha Brew Smoothie</h4>
                    <p class="text-gray-600"> vanilla | Dates | Banana | 100%
Cacao | Peanut Butter|
 Almond milk</p>
                    <span class="block mt-4 text-xl font-bold text-[#4caf50]">Regular ₹290 | Bowl ₹350</span>
                </div>
                <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105">
                    <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Smoothie" alt="Berry Bowl" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                    <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Berry Groove Smoothie </h4>
                    <p class="text-gray-600">Mixed berries, yogurt, and granola topped with fresh fruit.</p>
                    <span class="block mt-4 text-xl font-bold text-[#4caf50]">Regular ₹280 | Bowl ₹340</span>
                </div>
                <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105">
                    <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Frappe" alt="Fresh Juice" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                    <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Frappe Fravé</h4>
                    <p class="text-gray-600">Homemade Almond Butter | Espresso | Walnuts |
House Almond Milk | Vanilla Gelato</p>
                    <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹220</span>
                </div>
                <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105">
                    <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Frappe" alt="Fresh Juice" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                    <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Mocha Berry Fravé</h4>
                    <p class="text-gray-600">Espresso | Strawberries | Raspberries | Vanilla
Gelato | Milk | 100% Cacao</p>
                    <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹240</span>
                </div>
		<div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105">
                    <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Hot Chocolate" alt="Fresh Juice" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                    <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Cinnamon Drift Hot Chocolate</h4>
                    <p class="text-gray-600">100% Cacao | Milk Cinnamon | Nutmeg Organic
Jaggery</p>
                    <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹199</span>
                </div>
            </div>

            <!-- Pastas Section -->
            <h3 class="text-2xl font-semibold mb-4 text-[#1a4314] border-b-2 border-dashed border-[#4caf50] inline-block pb-1">Pastas</h3>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mt-4">
                <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105">
                    <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Pasta" alt="Avocado Toast" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                    <h4 class="font-bold text-xl mb-2 text-[#1a4314]">Red Ember Penne</h4>
                    <p class="text-gray-600">Penne Pasta | Inhouse Marinara Sauce | Zucchini | Bell Peppers | Mushrooms</p>
                    <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹320</span>
                </div>
                <div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105">
                    <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Pasta" alt="Quinoa Salad" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                    <h4 class="font-bold text-xl mb-2 text-[#1a4314]">White Viel Pasta</h4>
                    <p class="text-gray-600">Penne pasta | Béchamel Sauce | Mushrooms |
Parmesan | Truffle Oil</p>
                    <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹299</span>
                </div>
		<div class="bg-white rounded-lg shadow-lg p-6 transform transition duration-300 hover:scale-105">
                    <img src="https://placehold.co/200x200/d7c1b5/ffffff?text=Pasta" alt="Quinoa Salad" class="rounded-full w-24 h-24 mx-auto mb-4 object-cover">
                    <h4 class="font-bold text-xl mb-2 text-[#1a4314]">SPAGHETTI AGLIO E OLIO</h4>
                    <p class="text-gray-600">Spaghetti Pasta | Olive oil | Garlic | Parsley | Herbs</p>
                    <span class="block mt-4 text-xl font-bold text-[#4caf50]">₹289</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="bg-[#eaf4e5] py-16 px-4 md:px-8">
        <div class="max-w-4xl mx-auto text-center">
            <h2 class="text-3xl md:text-4xl font-bold mb-8 text-[#1a4314]">Get In Touch</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- Contact Form -->
                <div class="bg-white rounded-lg shadow-lg p-8">
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
                <div class="bg-white rounded-lg shadow-lg p-8 flex flex-col justify-center">
                    <h3 class="text-xl font-bold mb-4 text-[#1a4314]">Visit Us</h3>
                    <p class="text-gray-700 mb-2">258, Survey Nagar, Near Kalimata Mandir, Nagpur 440022</p>
                    <p class="text-gray-700 mb-2"><strong>Phone:</strong> +91 8087720122</p>
                    <p class="text-gray-700 mb-4"><strong>Email:</strong> frave@gmail.com</p>

                    <h3 class="text-xl font-bold mb-4 text-[#1a4314]">Hours of Operation</h3>
                    <p class="text-gray-700">Dine-In (12pm -10pm), Tuesdays Closed</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-[#1a4314] text-white py-8 px-4 md:px-8 text-center">
        <div class="max-w-6xl mx-auto">
            <p>&copy; 2025 Cafe Fravé. All Rights Reserved.</p>
            <div class="mt-4 flex justify-center space-x-4">
                <a href="#" class="hover:text-[#4caf50] transition duration-300">Facebook</a>
                <a href="https://www.instagram.com/frave.cafe/" class="hover:text-[#4caf50] transition duration-300">Instagram</a>
                <a href="#" class="hover:text-[#4caf50] transition duration-300">Twitter</a>
            </div>
        </div>
    </footer>

    <script>
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
