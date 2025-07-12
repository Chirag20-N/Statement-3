Problem Statement 3-ReWear – Community Clothing Exchange
Overview:
Develop ReWear, a web-based platform that enables users to exchange unused clothing
through direct swaps or a point-based redemption system. The goal is to promote sustainable
fashion and reduce textile waste by encouraging users to reuse wearable garments instead of
discarding them
Team Leader- Nakum Chirag , Mo:8160415162 , g-mail:nakumchirag244@gmail.com
Member 1- Yug Pathak , Mo:8849530573 , g-maill:Ymvpathak@gmail.om
Member 2-Pruthvish Naik , Mo:8141978791 g-mail:pruthvishnaik9@gmail.com

Code:
    <title>ReWear - Sustainable Clothing Exchange</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Poppins:wght@300;400;600;700&display=swap');
    :root {
        --primary: #3a7d44;
        --secondary: #d4af37;
        --accent: #ff7e5f;
    }
    body {
        font-family: 'Poppins', sans-serif;
    }
    h1, h2, h3, h4 {
        font-family: 'Playfair Display', serif;
    }
    .hero-gradient {
        background: linear-gradient(135deg, rgba(58, 125, 68, 0.9) 0%, rgba(212, 175, 55, 0.8) 100%);
    }
    .carousel-item {
        min-height: 400px;
    }
    .swap-card {
        transition: all 0.3s ease;
    }
    
    .swap-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 10px 25px rgba(0,0,0,0.1);
    }
    
    .auth-form {
        background: rgba(255,255,255,0.9);
        backdrop-filter: blur(10px);
    }
</style>
<section class="hero-gradient text-white py-20">
    <div class="container mx-auto px-4 flex flex-col md:flex-row items-center">
        <div class="md:w-1/2 mb-10 md:mb-0">
            <h1 class="text-4xl md:text-5xl font-bold mb-6">Swap Clothes, Not Waste</h1>
            <p class="text-xl mb-8">Join our sustainable fashion community to give pre-loved clothing a new life through swaps and points redemption.</p>
            <div class="flex flex-wrap gap-4">
                <button class="px-6 py-3 rounded-full bg-white text-green-700 font-medium hover:bg-gray-100 transition shadow-lg">Start Swapping</button>
                <button class="px-6 py-3 rounded-full bg-transparent border-2 border-white font-medium hover:bg-white hover:text-green-700 transition">How It Works</button>
            </div>
        </div>
        <div class="md:w-1/2 flex justify-center">
            <img src="Clothe.jpg" alt="Happy diverse group of people exchanging clothes in a park setting with trees in background" class="rounded-lg shadow-2xl">
        </div>
    </div>
</section>

<!-- How It Works Section -->
<section id="how-it-works" class="py-16 bg-white">
    <div class="container mx-auto px-4">
        <h2 class="text-3xl font-bold text-center mb-12">How ReWear Works</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div class="text-center p-6">
                <div class="bg-green-100 rounded-full w-24 h-24 flex items-center justify-center mx-auto mb-4">
                    <span class="text-4xl font-bold text-green-700">1</span>
                </div>
                <h3 class="text-xl font-semibold mb-3">List Your Items</h3>
                <p class="text-gray-600">Upload photos and details of the clothes you no longer wear but are still in good condition.</p>
            </div>
            <div class="text-center p-6">
                <div class="bg-green-100 rounded-full w-24 h-24 flex items-center justify-center mx-auto mb-4">
                    <span class="text-4xl font-bold text-green-700">2</span>
                </div>
                <h3 class="text-xl font-semibold mb-3">Browse & Select</h3>
                <p class="text-gray-600">Find items you'd love to wear from our community members across the country.</p>
            </div>
            <div class="text-center p-6">
                <div class="bg-green-100 rounded-full w-24 h-24 flex items-center justify-center mx-auto mb-4">
                    <span class="text-4xl font-bold text-green-700">3</span>
                </div>
                <h3 class="text-xl font-semibold mb-3">Exchange & Enjoy</h3>
                <p class="text-gray-600">Use points or direct swaps to get your new-to-you items shipped to your doorstep.</p>
            </div>
        </div>
    </div>
</section>

<!-- Featured Items Carousel -->
<section id="featured" class="py-16 bg-gray-50">
    <div class="container mx-auto px-4">
        <h2 class="text-3xl font-bold text-center mb-12">Featured Items Available</h2>
        <div class="relative overflow-hidden">
            <div class="flex transition-transform duration-300" id="carousel">
                <div class="carousel-item w-full md:w-1/3 flex-shrink-0 px-4">
                    <div class="swap-card bg-white rounded-lg overflow-hidden shadow-md">
                        <div class="relative h-64 overflow-hidden">
                            <img src="Jacket.jpg" alt="Vintage denim jacket with embroidered flowers on back in beige and blue colors" class="w-full h-full object-cover">
                            <span class="absolute top-4 right-4 bg-green-600 text-white text-xs px-2 py-1 rounded-full">Available</span>
                        </div>
                        <div class="p-4">
                            <div class="flex justify-between items-start mb-2">
                                <h3 class="font-semibold text-lg">Vintage Embroidered Denim Jacket</h3>
                                <span class="bg-green-100 text-green-800 text-xs px-2 py-1 rounded-full">Size M</span>
                            </div>
                            <p class="text-gray-600 text-sm mb-4">Light blue denim jacket with intricate floral embroidery on the back panels.</p>
                            <div class="flex justify-between items-center">
                                <span class="text-gray-900 font-medium">120 points</span>
                                <button class="text-green-600 hover:text-green-800 text-sm font-medium">View Details</button>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="carousel-item w-full md:w-1/3 flex-shrink-0 px-4">
                    <div class="swap-card bg-white rounded-lg overflow-hidden shadow-md">
                        <div class="relative h-64 overflow-hidden">
                            <img src="Bag.jpg" alt="Black leather crossbody bag with gold hardware and multiple compartments" class="w-full h-full object-cover">
                            <span class="absolute top-4 right-4 bg-green-600 text-white text-xs px-2 py-1 rounded-full">Available</span>
                        </div>
                        <div class="p-4">
                            <div class="flex justify-between items-start mb-2">
                                <h3 class="font-semibold text-lg">Classic Leather Crossbody Bag</h3>
                                <span class="bg-green-100 text-green-800 text-xs px-2 py-1 rounded-full">One Size</span>
                            </div>
                            <p class="text-gray-600 text-sm mb-4">Genuine black leather bag with adjustable strap and multiple inner pockets.</p>
                            <div class="flex justify-between items-center">
                                <span class="text-gray-900 font-medium">200 points</span>
                                <button class="text-green-600 hover:text-green-800 text-sm font-medium">View Details</button>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="carousel-item w-full md:1/3 flex-shrink-0 px-4">
                    <div class="swap-card bg-white rounded-lg overflow-hidden shadow-md">
                        <div class="relative h-64 overflow-hidden">
                            <img src="dress.jpg" alt="Linen wrap dress in navy blue with white polka dots and tie waist" class="w-full h-full object-cover">
                            <span class="absolute top-4 right-4 bg-green-600 text-white text-xs px-2 py-1 rounded-full">Available</span>
                        </div>
                        <div class="p-4">
                            <div class="flex justify-between items-start mb-2">
                                <h3 class="font-semibold text-lg">Polka Dot Linen Wrap Dress</h3>
                                <span class="bg-green-100 text-green-800 text-xs px-2 py-1 rounded-full">Size S</span>
                            </div>
                            <p class="text-gray-600 text-sm mb-4">Breathable linen dress perfect for summer with flattering wrap style.</p>
                            <div class="flex justify-between items-center">
                                <span class="text-gray-900 font-medium">150 points</span>
                                <button class="text-green-600 hover:text-green-800 text-sm font-medium">View Details</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <button class="absolute left-4 top-1/2 transform -translate-y-1/2 bg-white rounded-full p-2 shadow-md hover:bg-gray-100">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
                </svg>
            </button>
            <button class="absolute right-4 top-1/2 transform -translate-y-1/2 bg-white rounded-full p-2 shadow-md hover:bg-gray-100">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
                </svg>
            </button>
        </div>
        <div class="text-center mt-8">
            <button class="px-6 py-3 rounded-full bg-green-600 text-white font-medium hover:bg-green-700 transition shadow-lg">Browse All Items</button>
        </div>
    </div>
</section>

<!-- Benefits Section -->
<section id="benefits" class="py-16 bg-white">
    <div class="container mx-auto px-4">
        <h2 class="text-3xl font-bold text-center mb-12">Why Join ReWear</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
            <div class="flex">
                <div class="mr-6">
                    <div class="bg-green-100 rounded-full w-14 h-14 flex items-center justify-center">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-green-700" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z" />
                        </svg>
                    </div>
                </div>
                <div>
                    <h3 class="text-xl font-semibold mb-3">Sustainable Fashion</h3>
                    <p class="text-gray-600">Each item swapped prevents approximately 5kg of CO2 emissions from clothing production. Together we can significantly reduce fashion's environmental impact.</p>
                </div>
            </div>
            <div class="flex">
                <div class="mr-6">
                    <div class="bg-green-100 rounded-full w-14 h-14 flex items-center justify-center">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-green-700" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                        </svg>
                    </div>
                </div>
                <div>
                    <h3 class="text-xl font-semibold mb-3">Save Money</h3>
                    <p class="text-gray-600">Refresh your wardrobe without spending money. Our point system lets you earn value from items you no longer wear.</p>
                </div>
            </div>
            <div class="flex">
                <div class="mr-6">
                    <div class="bg-green-100 rounded-full w-14 h-14 flex items-center justify-center">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-green-700" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z" />
                        </svg>
                    </div>
                </div>
                <div>
                    <h3 class="text-xl font-semibold mb-3">Community Focused</h3>
                    <p class="text-gray-600">Connect with like-minded individuals who value sustainability. Our verification system ensures trust and accountability.</p>
                </div>
            </div>
            <div class="flex">
                <div class="mr-6">
                    <div class="bg-green-100 rounded-full w-14 h-14 flex items-center justify-center">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-green-700" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z" />
                        </svg>
                    </div>
                </div>
                <div>
                    <h3 class="text-xl font-semibold mb-3">Quality Assurance</h3>
                    <p class="text-gray-600">All items are vetted for quality before listing. We maintain standards so you receive items you'll love to wear.</p>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- CTA Section -->
<section class="py-16 bg-green-50">
    <div class="container mx-auto px-4 text-center">
        <h2 class="text-3xl font-bold mb-6">Ready to Start Swapping?</h2>
        <p class="text-xl text-gray-700 max-w-2xl mx-auto mb-8">Join our community of sustainable fashion enthusiasts today and give your wardrobe an eco-friendly refresh!</p>
        <div class="flex flex-wrap justify-center gap-4">
            <button class="px-8 py-3 rounded-full bg-green-600 text-white font-medium hover:bg-green-700 transition shadow-lg">Sign Up Now</button>
            <button class="px-8 py-3 rounded-full bg-white text-green-700 font-medium hover:bg-gray-100 transition border border-green-200">Take a Tour</button>
        </div>
    </div>
</section>

<!-- Footer -->
<footer class="bg-gray-900 text-white pt-16 pb-8">
    <div class="container mx-auto px-4">
        <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-12">
            <div>  
                <p class="text-gray-400">Making sustainable fashion accessible through community clothing exchange since 2023.</p>
            </div>
            <div>
                <h4 class="text-lg font-semibold mb-4">Quick Links</h4>
                <ul class="space-y-2">
                    <li><a href="#" class="text-gray-400 hover:text-white transition">How It Works</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-white transition">Browse Items</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-white transition">List an Item</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-white transition">FAQ</a></li>
                </ul>
            </div>
            <div>
                <h4 class="text-lg font-semibold mb-4">About Us</h4>
                <ul class="space-y-2">
                    <li><a href="#" class="text-gray-400 hover:text-white transition">Our Story</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-white transition">Sustainability Impact</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-white transition">Press</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-white transition">Careers</a></li>
                </ul>
            </div>
            <div>
                <h4 class="text-lg font-semibold mb-4">Connect</h4>
                <div class="flex space-x-4 mb-4">
                    <a href="#" class="bg-gray-800 hover:bg-gray-700 rounded-full w-10 h-10 flex items-center justify-center transition">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z" />
                        </svg>
                    </a>
                    <a href="#" class="bg-gray-800 hover:bg-gray-700 rounded-full w-10 h-10 flex items-center justify-center transition">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z" />
                        </svg>
                    </a>
                    <a href="#" class="bg-gray-800 hover:bg-gray-700 rounded-full w-10 h-10 flex items-center justify-center transition">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z" />
                        </svg>
                    </a>
                </div>
                <p class="text-gray-400 mb-2">contact@rewear.com</p>
                <p class="text-gray-400">+1 (555) 123-4567</p>
            </div>
        </div>
        <hr class="border-gray-700 mb-8">
        <div class="flex flex-col md:flex-row justify-between items-center text-gray-500 text-sm">
            <p>© 2023 ReWear Inc. All rights reserved.</p>
            <div class="flex space-x-4 mt-4 md:mt-0">
                <a href="#" class="hover:text-white transition">Privacy Policy</a>
                <a href="#" class="hover:text-white transition">Terms of Service</a>
            </div>
        </div>
    </div>
</footer>

<!-- Login Modal -->
<div class="fixed inset-0 bg-black bg-opacity-50 z-50 hidden items-center justify-center" id="loginModal">
    <div class="auth-form w-full max-w-md p-8 rounded-lg relative">
        <button class="absolute top-4 right-4 text-gray-500 hover:text-gray-700">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
            </svg>
        </button>
        <h3 class="text-2xl font-bold text-center mb-6">Welcome Back</h3>
        <form class="space-y-4">
            <div>
                <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email Address</label>
                <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="your@email.com">
            </div>
            <div>
                <label for="password" class="block text-sm font-medium text-gray-700 mb-1">Password</label>
                <input type="password" id="password" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-green-500 focus:border-transparent" placeholder="••••••••">
            </div>
            <div class="flex items-center justify-between">
                <div class="flex items-center">
                    <input id="remember-me" name="remember-me" type="checkbox" class="h-4 w-4 text-green-600 focus:ring-green-500 border-gray-300 rounded">
                    <label for="remember-me" class="ml-2 block text-sm text-gray-700">Remember me</label>
                </div>
                <a href="#" class="text-sm text-green-600 hover:text-green-800">Forgot password?</a>
            </div>
            <button type="submit" class="w-full py-3 bg-green-600 text-white rounded-lg hover:bg-green-700 focus:outline-none focus:ring-2 focus:ring-green-500 focus:ring-offset-2 transition">Sign In</button>
        </form>
        <p class="text-center text-sm mt-4 text-gray-600">Don't have an account? <a href="#" class="text-green-600 hover:text-green-800 font-medium">Sign up</a></p>
    </div>
</div>

<!-- Script for Carousel -->
<script>
    document.addEventListener('DOMContentLoaded', function() {
        const carousel = document.getElementById('carousel');
        const items = document.querySelectorAll('.carousel-item');
        const itemWidth = items[0].offsetWidth;
        let currentIndex = 0;
        
        function updateCarousel() {
            carousel.style.transform = `translateX(-${currentIndex * itemWidth}px)`;
        }
        
        document.querySelector('[aria-label="Previous"]').addEventListener('click', function() {
            currentIndex = (currentIndex > 0) ? currentIndex - 1 : items.length - 1;
            updateCarousel();
        });
        
        document.querySelector('[aria-label="Next"]').addEventListener('click', function() {
            currentIndex = (currentIndex < items.length - 1) ? currentIndex + 1 : 0;
            updateCarousel();
        });
        
        // Modal toggle
        const modal = document.getElementById('loginModal');
        document.querySelectorAll('[data-modal-toggle="loginModal"]').forEach(button => {
            button.addEventListener('click', function() {
                modal.classList.toggle('hidden');
                modal.classList.toggle('flex');
            });
        });
        
        document.querySelector('#loginModal button').addEventListener('click', function() {
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        });
    });
</script>
