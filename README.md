<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>The Solution Lab — Creative Solutions</title>
  <meta name="description" content="The Solution Lab — Creative services: design, branding, web & digital solutions." />
  <!-- Tailwind Play CDN (good for quick prototypes) -->
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    /* Custom colour palette for Red & White theme */
    :root{
      --brand-red:#e11d48; /* rose-600-ish */
      --brand-dark:#0f172a; /* slate-900 */
    }
    .brand-red{ background-color:var(--brand-red); }
    .brand-red-text{ color:var(--brand-red); }
    /* subtle glass effect for cards */
    .card-glass{ background-color: rgba(255,255,255,0.85); backdrop-filter: blur(6px); }
  </style>
</head>
<body class="antialiased text-slate-800 bg-white">
  <!-- NAV -->
  <header class="fixed w-full z-30 bg-white/80 backdrop-blur-sm shadow-sm">
    <div class="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
      <a href="#home" class="flex items-center gap-3">
        <div class="w-10 h-10 rounded-full flex items-center justify-center brand-red text-white font-bold">TS</div>
        <div>
          <div class="font-semibold">The Solution Lab</div>
          <div class="text-xs text-slate-500">Creative & Digital</div>
        </div>
      </a>

      <nav class="hidden md:flex gap-6 items-center text-sm">
        <a href="#home" class="hover:underline">Home</a>
        <a href="#about" class="hover:underline">About</a>
        <a href="#services" class="hover:underline">Services</a>
        <a href="#gallery" class="hover:underline">Gallery</a>
        <a href="#contact" class="hover:underline">Contact</a>
        <a href="#contact" class="ml-4 inline-block px-4 py-2 rounded-md font-medium brand-red text-white">Get Quote</a>
      </nav>

      <!-- Mobile menu button -->
      <button id="menuBtn" class="md:hidden p-2 rounded-md hover:bg-slate-100">
        <svg id="menuOpen" xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
        <svg id="menuClose" xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 hidden" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
        </svg>
      </button>
    </div>
    <!-- Mobile menu -->
    <div id="mobileMenu" class="md:hidden hidden px-6 pb-6">
      <div class="flex flex-col gap-3">
        <a href="#home" class="py-2">Home</a>
        <a href="#about" class="py-2">About</a>
        <a href="#services" class="py-2">Services</a>
        <a href="#gallery" class="py-2">Gallery</a>
        <a href="#contact" class="py-2">Contact</a>
      </div>
    </div>
  </header>

  <main class="pt-24">
    <!-- HERO -->
    <section id="home" class="relative overflow-hidden">
      <div class="max-w-6xl mx-auto px-6 py-20 lg:py-32 flex flex-col lg:flex-row items-center gap-12">
        <div class="w-full lg:w-1/2">
          <h1 class="text-4xl sm:text-5xl font-extrabold leading-tight">We build bold brands & beautiful digital experiences</h1>
          <p class="mt-4 text-lg text-slate-600">The Solution Lab helps startups and small businesses grow with creative design, branding, and websites that convert visitors into customers.</p>
          <div class="mt-8 flex gap-4">
            <a href="#contact" class="inline-block px-6 py-3 rounded-lg font-semibold brand-red text-white shadow-lg">Request a Quote</a>
            <a href="#services" class="inline-block px-6 py-3 rounded-lg border border-slate-200">Our Services</a>
          </div>

          <div class="mt-8 flex items-center gap-6">
            <div>
              <div class="text-sm text-slate-500">Clients served</div>
              <div class="text-2xl font-bold">120+</div>
            </div>
            <div>
              <div class="text-sm text-slate-500">Projects completed</div>
              <div class="text-2xl font-bold">350+</div>
            </div>
          </div>
        </div>

        <div class="w-full lg:w-1/2">
          <div class="card-glass rounded-2xl p-6 shadow-xl">
            <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?q=80&w=1200&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="creative" class="w-full rounded-lg object-cover h-64 sm:h-80" />
            <div class="mt-4">
              <h3 class="font-semibold">Creative process that works</h3>
              <p class="text-sm text-slate-600 mt-2">Discovery → Strategy → Design → Delivery. We partner with you at every step, keeping things simple and effective.</p>
            </div>
          </div>
        </div>
      </div>
      <!-- decorative SVG -->
      <div class="absolute right-0 top-0 opacity-5 pointer-events-none">
        <svg width="400" height="400" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
          <circle cx="100" cy="100" r="80" fill="var(--brand-red)" />
        </svg>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="about" class="max-w-6xl mx-auto px-6 py-16">
      <div class="grid grid-cols-1 lg:grid-cols-3 gap-8 items-center">
        <div class="lg:col-span-2">
          <h2 class="text-3xl font-bold">About The Solution Lab</h2>
          <p class="mt-4 text-slate-600">We are a creative studio focused on delivering memorable brands and effective digital products. Our team blends design thinking with practical engineering to create solutions that drive results.</p>

          <ul class="mt-6 grid grid-cols-1 sm:grid-cols-2 gap-4">
            <li class="flex gap-3 items-start">
              <div class="w-10 h-10 rounded-full brand-red text-white flex items-center justify-center font-semibold">1</div>
              <div>
                <div class="font-semibold">Design-first thinking</div>
                <div class="text-sm text-slate-600">User experience is at the heart of everything we build.</div>
              </div>
            </li>
            <li class="flex gap-3 items-start">
              <div class="w-10 h-10 rounded-full brand-red text-white flex items-center justify-center font-semibold">2</div>
              <div>
                <div class="font-semibold">Fast delivery</div>
                <div class="text-sm text-slate-600">Lean sprints so you launch sooner and iterate faster.</div>
              </div>
            </li>
          </ul>
        </div>
        <div class="hidden lg:block">
          <div class="rounded-xl overflow-hidden shadow-lg">
            <img src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d?q=80&w=800&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="studio" class="w-full h-full object-cover" />
          </div>
        </div>
      </div>
    </section>

    <!-- SERVICES -->
    <section id="services" class="bg-slate-50 py-16">
      <div class="max-w-6xl mx-auto px-6">
        <h2 class="text-3xl font-bold">Services</h2>
        <p class="mt-2 text-slate-600">Services built for growth — mix and match as per your needs.</p>

        <div class="mt-8 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
          <div class="p-6 rounded-lg card-glass shadow">
            <div class="text-3xl font-bold brand-red-text">Branding</div>
            <p class="mt-3 text-sm text-slate-600">Logo, visual identity, brand guidelines, and messaging that stands out.</p>
          </div>
          <div class="p-6 rounded-lg card-glass shadow">
            <div class="text-3xl font-bold brand-red-text">Web Design</div>
            <p class="mt-3 text-sm text-slate-600">Responsive websites, landing pages, and microsites optimized for conversion.</p>
          </div>
          <div class="p-6 rounded-lg card-glass shadow">
            <div class="text-3xl font-bold brand-red-text">Digital Marketing</div>
            <p class="mt-3 text-sm text-slate-600">Social ads, SEO basics, and campaigns to get your message in front of the right people.</p>
          </div>
          <div class="p-6 rounded-lg card-glass shadow">
            <div class="text-3xl font-bold brand-red-text">UI/UX</div>
            <p class="mt-3 text-sm text-slate-600">User flows, prototypes, and usability testing for better engagement.</p>
          </div>
          <div class="p-6 rounded-lg card-glass shadow">
            <div class="text-3xl font-bold brand-red-text">E-commerce</div>
            <p class="mt-3 text-sm text-slate-600">Product catalogs, checkout flows and integrations to scale sales.</p>
          </div>
          <div class="p-6 rounded-lg card-glass shadow">
            <div class="text-3xl font-bold brand-red-text">Maintenance</div>
            <p class="mt-3 text-sm text-slate-600">Ongoing support, updates and performance monitoring.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- GALLERY -->
    <section id="gallery" class="max-w-6xl mx-auto px-6 py-16">
      <h2 class="text-3xl font-bold">Gallery</h2>
      <p class="mt-2 text-slate-600">Some recent work & snapshots from client projects.</p>

      <div class="mt-6 grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-4 gap-4">
        <!-- Use placeholders; replace with your images -->
        <img class="w-full h-40 object-cover rounded-lg shadow" src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?q=80&w=600&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="gallery1" />
        <img class="w-full h-40 object-cover rounded-lg shadow" src="https://images.unsplash.com/photo-1504639725590-34d0984388bd?q=80&w=600&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="gallery2" />
        <img class="w-full h-40 object-cover rounded-lg shadow" src="https://images.unsplash.com/photo-1492724441997-5dc865305da7?q=80&w=600&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="gallery3" />
        <img class="w-full h-40 object-cover rounded-lg shadow" src="https://images.unsplash.com/photo-1522204508391-0b9d0a7ddf3b?q=80&w=600&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="gallery4" />
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="bg-white py-16 border-t">
      <div class="max-w-4xl mx-auto px-6">
        <h2 class="text-3xl font-bold">Contact</h2>
        <p class="mt-2 text-slate-600">Ready to start? Tell us a bit about your project and we'll get back to you.</p>

        <div class="mt-6 grid grid-cols-1 md:grid-cols-2 gap-6">
          <form class="space-y-4" action="https://formspree.io/f/your-form-id" method="POST">
            <div>
              <label class="block text-sm font-medium">Name</label>
              <input name="name" required class="mt-1 block w-full rounded-md border border-slate-200 px-3 py-2" />
            </div>
            <div>
              <label class="block text-sm font-medium">Email</label>
              <input name="email" type="email" required class="mt-1 block w-full rounded-md border border-slate-200 px-3 py-2" />
            </div>
            <div class="md:col-span-2">
              <label class="block text-sm font-medium">Message</label>
              <textarea name="message" rows="5" required class="mt-1 block w-full rounded-md border border-slate-200 px-3 py-2"></textarea>
            </div>
            <div>
              <button type="submit" class="px-6 py-3 rounded-lg brand-red text-white font-semibold">Send Message</button>
            </div>
          </form>

          <div class="flex flex-col gap-4">
            <div class="p-4 rounded-lg shadow card-glass">
              <div class="font-semibold">Office</div>
              <div class="text-sm text-slate-600 mt-1">123, Creative Street, Your City</div>
            </div>
            <div class="p-4 rounded-lg shadow card-glass">
              <div class="font-semibold">Email</div>
              <div class="text-sm text-slate-600 mt-1">hello@thesolutionlab.example</div>
            </div>
            <div class="p-4 rounded-lg shadow card-glass">
              <div class="font-semibold">Phone</div>
              <div class="text-sm text-slate-600 mt-1">+91 98765 43210</div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-slate-900 text-white mt-12">
      <div class="max-w-6xl mx-auto px-6 py-8 flex flex-col md:flex-row justify-between items-center gap-4">
        <div>
          <div class="font-semibold">The Solution Lab</div>
          <div class="text-sm text-slate-400">© " + new Date().getFullYear() + " All rights reserved.</div>
        </div>
        <div class="flex gap-4">
          <a href="#" aria-label="twitter" class="text-slate-300 hover:text-white">Twitter</a>
          <a href="#" aria-label="linkedin" class="text-slate-300 hover:text-white">LinkedIn</a>
          <a href="#" aria-label="instagram" class="text-slate-300 hover:text-white">Instagram</a>
        </div>
      </div>
    </footer>
  </main>

  <script>
    // Mobile menu toggle
    const menuBtn = document.getElementById('menuBtn');
    const mobileMenu = document.getElementById('mobileMenu');
    const menuOpen = document.getElementById('menuOpen');
    const menuClose = document.getElementById('menuClose');
    menuBtn && menuBtn.addEventListener('click', ()=>{
      mobileMenu.classList.toggle('hidden');
      menuOpen.classList.toggle('hidden');
      menuClose.classList.toggle('hidden');
    });

    // Smooth scroll for internal links
    document.querySelectorAll('a[href^="#"]').forEach(anchor=>{
      anchor.addEventListener('click', function(e){
        const target = document.querySelector(this.getAttribute('href'));
        if(target){ e.preventDefault(); target.scrollIntoView({ behavior: 'smooth', block: 'start' }); }
      });
    });
  </script>
</body>
</html>
